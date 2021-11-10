# image-lambda

## Author

Antoine Charette

## Problem Domain

In this lab we are tasked with making a lambda function that saves files to an s3 bucket and is able to view s3 buckets. The public access should be read only.

## Process

The Lambda function will be triggered by actions being made in the images S3 bucket. It will take information in from the bucket and then update the images.json file. If there is no images.json file, it creates on with the bucket info.

My AWS has a terrible bug that I have been trying to fix for the past few days. I cant read anything from the S3 bucket so my images.json file is full of {type: 'image'}. It seems to be adding more than needed and it is not able to add the information from the files added because of this glitch.
