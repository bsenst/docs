---
title: Network troubleshooting
weight: 2
tags:
- troubleshooting
- networking
description: >
  How to troubleshoot common network problems
---

## Overview

Below are several scenarios in which you may be trying to use LocalStack.
If you are having difficulties connecting your application code to LocalStack, please visit the links below each section which go into further details.

---

## Accessing LocalStack directly using HTTP

{{< figure src="./images/overview-1.png" width="400" >}}

You are trying to reach LocalStack directly via endpoint directly, for example with the [AWS CLI]({{< ref "user-guide/integrations/aws-cli" >}}), and need to specify the URL of LocalStack yourself, such as:

{{< command >}}
aws --endpoint-url http://localhost.localstack.cloud:4566 <command>
# or
awslocal <command>
{{< / command >}}

[Click here to learn more...]({{< ref "endpoint-url" >}})

## Accessing LocalStack using a language SDK

{{< figure src="./images/overview-2.png" width="400" >}}

You are using a [language SDK]({{< ref "/user-guide/integrations/sdks" >}}) to access LocalStack, for example [`boto3`](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) or the [`go`](https://github.com/aws/aws-sdk-go-v2) SDK.

[Click here to learn more...]({{< ref "sdk" >}})

## Accessing a resource that LocalStack has created by URL

{{< figure src="./images/overview-3.png" width="400" >}}

You have created a resource in LocalStack such as an RDS or OpenSearch instance.

[Click here to learn more...]({{< ref "created-resources" >}})