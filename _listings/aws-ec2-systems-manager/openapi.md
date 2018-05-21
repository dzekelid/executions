---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 1
info:
  title: AWS EC2 Systems Manager API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeAutomationExecutions:
    get:
      summary: Describe Automation Executions
      description: Provides details about all active and terminated Automation executions.
      operationId: describeAutomationExecutions
      x-api-path-slug: actiondescribeautomationexecutions-get
      parameters:
      - in: query
        name: Filters
        description: Filters used to limit the scope of executions that are requested
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        apps:
          description: app_allow
        devices:
          description: device_link
        members:
          description: member_invite
        passwords:
          description: tfa_enable
        sharing:
          description: shmodel_create
        team_admin_actions:
          description: sf_external_accept_allow
        200:
          description: OK
      tags:
      - Automation
      - Executions
  /?Action=DescribeMaintenanceWindowExecutions:
    get:
      summary: Describe Maintenance Window Executions
      description: |-
        Lists the executions of a Maintenance Window (meaning, information about when the
           Maintenance Window was scheduled to be active and information about tasks registered and run with
           the Maintenance Window).
      operationId: describeMaintenanceWindowExecutions
      x-api-path-slug: actiondescribemaintenancewindowexecutions-get
      parameters:
      - in: query
        name: Filters
        description: 'Each entry in the array is a structure containing:'
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: WindowId
        description: The ID of the Maintenance Window whose executions should be retrieved
        type: string
      responses:
        200:
          description: OK
      tags:
      - Maintenance
      - Window
      - Executions
---