---
name: SmartBear Software
description: SmartBear Software provides tools for over 100,000 software professionals
  to build, test, and monitor some of the best software applications and websites
  anywhere on the desktop, mobile and in the cloud.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/SmartBear-Logo.png
x-kinRank: "9"
x-alexaRank: ""
tags:
- Virtualization
- Testing
- Stack Network
- Security
- Performance
- Monitoring
- API LIfeycle
created: "2018-03-23"
modified: "2018-03-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/executions/master/_listings/smartbear-software/apis.yaml
specificationVersion: "0.14"
apis:
- name: TestServer REST API
  description: SmartBear Software provides tools for over 100,000 software professionals
    to build, test, and monitor some of the best software applications and websites
    anywhere on the desktop, mobile and in the cloud
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/SmartBear-Logo.png
  humanURL: ""
  baseURL: ://testserver.readyapi.io:8080//v1
  tags: Executions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/executions/master/_listings/smartbear-software/readyapi-executions-executionid-transactions-transactionid-get.md
- name: TestServer REST API Posts a file for the specified test run
  description: Use this operation to send additional files required by the executed
    test recipes. For example, you may need to send an Excel file for your test recipe
    that uses an Excel data source. The test recipe will be in the "PENDING" status
    until it receives the required file. Use the <code>multipart/form-data</code>
    media type for this request.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/SmartBear-Logo.png
  humanURL: http://smartbear.com/
  baseURL: http:://testserver.readyapi.io:8080//v1
  tags: Executions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/executions/master/_listings/smartbear-software/readyapi-executions-executionid-files-post.md
x-common:
- type: x-blog
  url: http://blog.smartbear.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/smartbear
- type: x-crunchbase
  url: http://www.crunchbase.com/company/smart-bear-software
- type: x-github
  url: https://github.com/SmartBear
- type: x-twitter
  url: https://twitter.com/smartbear
- type: x-website
  url: http://smartbear.com/
- type: x-blog
  url: http://blog.smartbear.com/
- type: x-blog-rss
  url: http://feeds.feedburner.com/smartbear
- type: x-crunchbase
  url: http://www.crunchbase.com/company/smart-bear-software
- type: x-github
  url: https://github.com/SmartBear
- type: x-twitter
  url: https://twitter.com/smartbear
- type: x-website
  url: http://smartbear.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---