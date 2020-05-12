# Delete DynamoDB table


## Document Design

Refer to schema.json

Document Steps:
1. aws:executeScript - Delete DynamoDB table
   * Inputs:
     * Runtime: python3.6
     * Handler: script_handler
     * Script: Python script that runs the code
     * InputPayload:
       * TableName: {{TableName}} - Name of the DynamoDB table

## Test script

Test will:
  1. Create a test stack with a single DynamoDB table
  2. Execute automation document to delete the DynamoDB table
  3. Ensure the automation has executed successfully
  4. Clean up test stack
