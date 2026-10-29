# AWS Lambda + API Gateway — Serverless Student API

## Project Overview

This project demonstrates a serverless REST API using Amazon API Gateway and AWS Lambda. The API returns student information in JSON format without requiring a continuously running EC2 server.

## Architecture

Client → Amazon API Gateway → AWS Lambda → JSON Response

## AWS Services Used

- AWS Lambda — Executes Python backend code
- Amazon API Gateway — Exposes the HTTP endpoint
- AWS IAM — Manages permissions
- Amazon CloudWatch — Stores execution logs

## Features

- Serverless API endpoint
- Python-based Lambda function
- HTTP GET request handling
- JSON response
- CloudWatch logging and troubleshooting

## Sample Response

```json
{
  "id": 101,
  "name": "Meghana",
  "course": "AWS DevOps"
}
```

## Deployment Steps

1. Create a Python Lambda function.
2. Deploy the function code.
3. Create an HTTP API in Amazon API Gateway.
4. Configure the `GET /students` route.
5. Connect the route to the Lambda function.
6. Deploy the API and test the Invoke URL.
7. Review execution logs in CloudWatch.

## Security

- Follow the principle of least privilege for IAM permissions.
- Do not commit AWS credentials or sensitive data.
- Add authentication and authorization before exposing sensitive information.

## Learning Outcomes

- Understanding serverless architecture
- Integrating API Gateway with Lambda
- Working with HTTP methods and JSON responses
- Troubleshooting Lambda execution and API errors
