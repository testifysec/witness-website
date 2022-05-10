---
title: "AWS Instance Identity"
linkTitle: "AWS Instance Identity"
date: 2022-05-01
description: "Attest that a command was executed on an AWS instance you trust"
---

The AWS (Amazon Web Services) Instance Identity Attestor communicates with the AWS Instance Metadata to collect
information about the AWS instance Witness on which executing. The document signature is
verified with the AWS RSA public certificate available [here](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/verify-signature.html).
This verification method currently does not work for the Hong Kong, Bahrain, Cape Town, Milan, China, or
GovCloud regions.

## Subjects

| Subject | Description |
| ------- | ----------- |
| `instanceid` | The ID of the AWS instance where Witness was executed |
| `accountid` | ID of the account that owns the AWS instance |
| `imageid` | ID of the AMI ([Amazon Machine Image](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AMIs.html)) the instance was running at time of execution |
| `privateip` | IP address of the instance at time of execution |
