# AWSPublicIPAddressRanges

## Introduction

This repo tracks the changes made to the official AWS IP Address Range list available on [https://ip-ranges.amazonaws.com/ip-ranges.json](https://ip-ranges.amazonaws.com/ip-ranges.json)

More details about the content are documented on [docs.aws.amazon.com](http://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html)

## Usage examples

Since AWS publishes a json file it is easy to filter using tools like [jq](https://stedolan.github.io/jq/). AWS published some good examples on [docs.aws.amazon.com](http://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html)

## AWS IP address range notifications

Instead of consuming the json file or this git repo, you can also subscribe to the AWS SNS topic _arn:aws:sns:us-east-1:806199016981:AmazonIpSpaceChanged_ as documented on [docs.aws.amazon.com](http://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html)
