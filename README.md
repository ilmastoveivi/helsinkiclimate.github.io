## About the project

This repository is used for the development of the https://helsinkiclimate.org website for the Helsinki Climate event related to the Ilmastoveivi2019 campaign. The purpose of the website is to work as a simple landing page for people to be able to subscribe for emails related to the event/campaign. You can read more about the campaign here: https://ilmastoveivi2019.fi/campaign.

## How to participate

The page uses Jekyll and is hosted by AWS S3. You can test the website locally on your computer by following the instructions on the Jekyll website: https://jekyllrb.com/

Instructions for Windows and MacOS:
- https://jekyllrb.com/docs/installation/windows/
- https://jekyllrb.com/docs/installation/macos/

You are welcome to participate in the development for example by contacting the campaign team.

## Deployment

Deployment is currently done manually with the s3_website tool: https://github.com/laurilehmijoki/s3_website. Currently only Gofore Crew members may obtain access to deploy, since the S3 bucket where the website is hosted is owned by Gofore Crew. To be able to deploy to S3, you require AWS credentials and acquired access keys for Gofore Crew. After acquiring them, you need to insert the keys in a file named `credentials` in `.aws`-folder located in your system user's home folder. The file content must be given in format:

```
[default]
aws_access_key_id = <YOUR_AWS_ACCESS_KEY_ID_HERE>
aws_secret_access_key = <YOUR_AWS_SECRET_ACCESS_KEY_HERE>
```

After saving the credentials-file, you should now be able to deploy to S3 with the CLI command: `s3_website push`.

## Contacts

- info@ilmastoveivi2019.fi
- https://twitter.com/Ilmastoveivi19
- https://www.facebook.com/ilmastoveivi2019
- https://www.instagram.com/ilmastoveivi2019/

## License

Graphics and images of the campaign are copyright of Luka Appelberg. Blog posts are copyright of their authors. Logos and other images of the participating organizations are copyright of the respective organizations. 

The source code can be used according to the MIT license below:

Copyright 2019 Ilmastoveivaajat ry. 

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
