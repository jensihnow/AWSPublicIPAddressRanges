# AWSPublicIPAddressRanges

## Introduction

This repo tracks the changes made to the official AWS IP Address Range list available on [https://ip-ranges.amazonaws.com/ip-ranges.json](https://ip-ranges.amazonaws.com/ip-ranges.json).

Please see official documentation for guidance on: [https://docs.aws.amazon.com/](https://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html).


## Content syntax

Please see syntax on the official documentation on [docs.aws.amazon.com](https://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html#aws-ip-syntax)

## Usage examples

Since AWS publishes a json file it is easy to filter using tools like [jq](https://stedolan.github.io/jq/). AWS published some good examples on [docs.aws.amazon.com](http://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html)

## AWS IP address range notifications

Instead of consuming the json file or this git repo, you can also subscribe to the AWS SNS topic _arn:aws:sns:us-east-1:806199016981:AmazonIpSpaceChanged_ as documented on [docs.aws.amazon.com](http://docs.aws.amazon.com/general/latest/gr/aws-ip-ranges.html)

## About

As AWS is only keeping the current state it becomes hard to track changes over time. Comparing a saved state with a new one is easy using the publication time, as long as you have a previous file saved.

This repo is updated once a day, by automation, which allows to track changes on a daily basis and compare using git/diff tools.