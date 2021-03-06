---
swagger: "2.0"
info:
  title: TestServer REST API Runs a test recipe.
  description: Use this operation to send a test recipe to the TestServer. The recipe
    contents is passed in the request body (should be valid JSON contents).
  contact:
    name: SmartBear Software
    url: http://smartbear.com/testserver
  version: 1.2.1
host: testserver.readyapi.io:8080
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /readyapi/executions:
    post:
      summary: Runs a test recipe.
      description: Use this operation to send a test recipe to the TestServer
      operationId: postRecipe
      parameters:
      - in: query
        name: async
        description: Specifies when the TestServer replies:<br/>`true` - Immediately
      - in: body
        name: body
        description: JSON-based test recipe contents
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: callback
        description: The URL, to which the results will be posted
      responses:
        200:
          description: OK
      tags:
      - executions
definitions:
  MultiPart:
    properties:
      entity:
        description: This is a default description.
        type: string
      headers:
        description: This is a default description.
        type: string
      bodyParts:
        description: This is a default description.
        type: string
      parameterizedHeaders:
        description: This is a default description.
        type: string
  MediaType:
    properties:
      type:
        description: This is a default description.
        type: string
      subtype:
        description: This is a default description.
        type: string
      parameters:
        description: This is a default description.
        type: string
      wildcardType:
        description: This is a default description.
        type: string
      wildcardSubtype:
        description: This is a default description.
        type: string
  ProjectResultReport:
    properties:
      projectName:
        description: This is a default description.
        type: string
      status:
        description: This is a default description.
        type: string
      testSuiteResultReports:
        description: This is a default description.
        type: string
      timeTaken:
        description: This is a default description.
        type: string
      startTime:
        description: This is a default description.
        type: string
      executionID:
        description: This is a default description.
        type: string
      unresolvedFiles:
        description: This is a default description.
        type: string
  UnresolvedFile:
    properties:
      fileName:
        description: This is a default description.
        type: string
  FormDataBodyPart:
    properties:
      entity:
        description: This is a default description.
        type: string
      headers:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
      value:
        description: This is a default description.
        type: string
      simple:
        description: This is a default description.
        type: string
      parameterizedHeaders:
        description: This is a default description.
        type: string
  Authentication:
    properties:
      type:
        description: This is a default description.
        type: string
      username:
        description: This is a default description.
        type: string
      password:
        description: This is a default description.
        type: string
      domain:
        description: This is a default description.
        type: string
      accessToken:
        description: This is a default description.
        type: string
      accessTokenPosition:
        description: This is a default description.
        type: string
      accessTokenUri:
        description: This is a default description.
        type: string
      clientId:
        description: This is a default description.
        type: string
      clientSecret:
        description: This is a default description.
        type: string
      refreshToken:
        description: This is a default description.
        type: string
  TestStepResultReport:
    properties:
      testStepName:
        description: This is a default description.
        type: string
      assertionStatus:
        description: This is a default description.
        type: string
      timeTaken:
        description: This is a default description.
        type: string
      transactionId:
        description: This is a default description.
        type: string
      messages:
        description: This is a default description.
        type: string
  DataSource:
    properties:
      properties:
        description: This is a default description.
        type: string
      grid:
        description: This is a default description.
        type: string
  PropertyTransferTarget:
    properties:
      targetName:
        description: This is a default description.
        type: string
      property:
        description: This is a default description.
        type: string
      pathLanguage:
        description: This is a default description.
        type: string
      path:
        description: This is a default description.
        type: string
  PropertyTransferSource:
    properties:
      sourceName:
        description: This is a default description.
        type: string
      property:
        description: This is a default description.
        type: string
      pathLanguage:
        description: This is a default description.
        type: string
      path:
        description: This is a default description.
        type: string
  TestStep:
    properties:
      type:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
  FileDataSource:
    properties:
      file:
        description: This is a default description.
        type: string
      charset:
        description: This is a default description.
        type: string
      separator:
        description: This is a default description.
        type: string
      trim:
        description: This is a default description.
        type: string
      quotedValues:
        description: This is a default description.
        type: string
  FormDataMultiPart:
    properties:
      entity:
        description: This is a default description.
        type: string
      headers:
        description: This is a default description.
        type: string
      bodyParts:
        description: This is a default description.
        type: string
      fields:
        description: This is a default description.
        type: string
      parameterizedHeaders:
        description: This is a default description.
        type: string
  TestCaseResultReport:
    properties:
      testCaseName:
        description: This is a default description.
        type: string
      testStepResultReports:
        description: This is a default description.
        type: string
  RestParameter:
    properties:
      type:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
      value:
        description: This is a default description.
        type: string
  SoapParameter:
    properties:
      name:
        description: This is a default description.
        type: string
      path:
        description: This is a default description.
        type: string
      value:
        description: This is a default description.
        type: string
  FormDataContentDisposition:
    properties:
      type:
        description: This is a default description.
        type: string
      parameters:
        description: This is a default description.
        type: string
      fileName:
        description: This is a default description.
        type: string
      creationDate:
        description: This is a default description.
        type: string
      modificationDate:
        description: This is a default description.
        type: string
      readDate:
        description: This is a default description.
        type: string
      size:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
  ParameterizedHeader:
    properties:
      value:
        description: This is a default description.
        type: string
      parameters:
        description: This is a default description.
        type: string
  PropertyTransfer:
    properties:
      transferName:
        description: This is a default description.
        type: string
      failTransferOnError:
        description: This is a default description.
        type: string
      setNullOnMissingSource:
        description: This is a default description.
        type: string
      transferTextContent:
        description: This is a default description.
        type: string
      ignoreEmptyValue:
        description: This is a default description.
        type: string
      transferToAll:
        description: This is a default description.
        type: string
      transferChildNodes:
        description: This is a default description.
        type: string
      entitizeTransferredValues:
        description: This is a default description.
        type: string
  ExcelDataSource:
    properties:
      file:
        description: This is a default description.
        type: string
      worksheet:
        description: This is a default description.
        type: string
      startAtCell:
        description: This is a default description.
        type: string
      ignoreEmpty:
        description: This is a default description.
        type: string
  ProjectResultReports:
    properties:
      projectResultReports:
        description: This is a default description.
        type: string
  Assertion:
    properties:
      type:
        description: This is a default description.
        type: string
      name:
        description: This is a default description.
        type: string
  ContentDisposition:
    properties:
      type:
        description: This is a default description.
        type: string
      parameters:
        description: This is a default description.
        type: string
      fileName:
        description: This is a default description.
        type: string
      creationDate:
        description: This is a default description.
        type: string
      modificationDate:
        description: This is a default description.
        type: string
      readDate:
        description: This is a default description.
        type: string
      size:
        description: This is a default description.
        type: string
  BodyPart:
    properties:
      entity:
        description: This is a default description.
        type: string
      headers:
        description: This is a default description.
        type: string
      parameterizedHeaders:
        description: This is a default description.
        type: string
  TestCase:
    properties:
      searchProperties:
        description: This is a default description.
        type: string
      maintainSession:
        description: This is a default description.
        type: string
      abortOnError:
        description: This is a default description.
        type: string
      failTestCaseOnError:
        description: This is a default description.
        type: string
      discardOkResults:
        description: This is a default description.
        type: string
      socketTimeout:
        description: This is a default description.
        type: string
      testCaseTimeout:
        description: This is a default description.
        type: string
      clientCertFileName:
        description: This is a default description.
        type: string
      clientCertPassword:
        description: This is a default description.
        type: string
      testSteps:
        description: This is a default description.
        type: string
  TestSuiteResultReport:
    properties:
      testSuiteName:
        description: This is a default description.
        type: string
      testCaseResultReports:
        description: This is a default description.
        type: string
  HarLogRoot:
    properties: []
  HarLog:
    properties:
      version:
        description: This is a default description.
        type: string
      pages:
        description: This is a default description.
        type: string
      entries:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarCreator:
    properties:
      name:
        description: This is a default description.
        type: string
      version:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarBrowser:
    properties:
      name:
        description: This is a default description.
        type: string
      version:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarPage:
    properties:
      startedDateTime:
        description: This is a default description.
        type: string
      id:
        description: This is a default description.
        type: string
      title:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarPageTimings:
    properties:
      onContentLoad:
        description: This is a default description.
        type: string
      onLoad:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarEntry:
    properties:
      pageref:
        description: This is a default description.
        type: string
      startedDateTime:
        description: This is a default description.
        type: string
      time:
        description: This is a default description.
        type: string
      serverIPAddress:
        description: This is a default description.
        type: string
      connection:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarRequest:
    properties:
      method:
        description: This is a default description.
        type: string
      url:
        description: This is a default description.
        type: string
      httpVersion:
        description: This is a default description.
        type: string
      cookies:
        description: This is a default description.
        type: string
      headers:
        description: This is a default description.
        type: string
      queryString:
        description: This is a default description.
        type: string
      headersSize:
        description: This is a default description.
        type: string
      bodySize:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarResponse:
    properties:
      status:
        description: This is a default description.
        type: string
      statusText:
        description: This is a default description.
        type: string
      httpVersion":
        description: This is a default description.
        type: string
      cookies:
        description: This is a default description.
        type: string
      headers:
        description: This is a default description.
        type: string
      redirectURL:
        description: This is a default description.
        type: string
      headersSize:
        description: This is a default description.
        type: string
      bodySize:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarCache:
    properties:
      comment:
        description: This is a default description.
        type: string
  HarTimings:
    properties:
      blocked:
        description: This is a default description.
        type: string
      dns:
        description: This is a default description.
        type: string
      connect:
        description: This is a default description.
        type: string
      send:
        description: This is a default description.
        type: string
      wait:
        description: This is a default description.
        type: string
      receive:
        description: This is a default description.
        type: string
      ssl:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarCookie:
    properties:
      name:
        description: This is a default description.
        type: string
      value:
        description: This is a default description.
        type: string
      path:
        description: This is a default description.
        type: string
      domain:
        description: This is a default description.
        type: string
      expires:
        description: This is a default description.
        type: string
      httpOnly:
        description: This is a default description.
        type: string
      secure:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarHeader:
    properties:
      name:
        description: This is a default description.
        type: string
      value:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarContent:
    properties:
      size:
        description: This is a default description.
        type: string
      compression:
        description: This is a default description.
        type: string
      mimeType:
        description: This is a default description.
        type: string
      text:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarQueryString:
    properties:
      name:
        description: This is a default description.
        type: string
      value:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarCacheRequest:
    properties:
      expires:
        description: This is a default description.
        type: string
      lastAccess:
        description: This is a default description.
        type: string
      hitCount:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
      etag:
        description: This is a default description.
        type: string
  HarPostData:
    properties:
      mimeType:
        description: This is a default description.
        type: string
      params:
        description: This is a default description.
        type: string
      text:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  HarParam:
    properties:
      name:
        description: This is a default description.
        type: string
      value:
        description: This is a default description.
        type: string
      fileName:
        description: This is a default description.
        type: string
      contentType:
        description: This is a default description.
        type: string
      comment:
        description: This is a default description.
        type: string
  DataGenDataSource:
    properties:
      numberOfRows:
        description: This is a default description.
        type: string
      dataGenerators:
        description: This is a default description.
        type: string
  DataGenerator:
    properties:
      type:
        description: This is a default description.
        type: string
      propertyName:
        description: This is a default description.
        type: string
      duplicationFactor:
        description: This is a default description.
        type: string
x-collection-name: SmartBear Software
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---