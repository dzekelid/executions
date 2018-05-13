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
- name: TestServer REST API Cancels the specified recipe execution
  description: Use this operation to stop the run specified by <i>executionID</i>.
    You can find in the response to your execution request ([see how](http://readyapi.smartbear.com/testserver/tutorials/your_first_recipe/results)),
    or you can send a GET <code>/readyapi/executions</code> request to the TestServer.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/SmartBear-Logo.png
  humanURL: http://smartbear.com/
  baseURL: http:://testserver.readyapi.io:8080//v1
  tags: Executions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/executions/master/_listings/smartbear-software/readyapi-executions-executionid-delete.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/executions/master/_listings/smartbear-software/readyapi-executions-executionid-delete-postman.md
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