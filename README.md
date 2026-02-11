# MarkForge Notification Service

MarkForge Notification Service manages event driven alerts and system notifications across the platform.

It delivers updates related to document edits, version changes, export completion, and administrative actions.

## Responsibilities

- Store user notifications
- Deliver real time alerts
- Track document related events
- Mark notifications as read
- Provide notification retrieval APIs

## Architecture

Fully serverless AWS architecture:

- AWS Lambda (business logic)
- Amazon DynamoDB (notification storage)
- Amazon API Gateway (REST or WebSocket API)
- Amazon EventBridge (optional event triggers)
- AWS IAM for secure permissions

## Event Flow

1. Document or export event occurs
2. Event triggers Lambda function
3. Notification stored in DynamoDB
4. Frontend retrieves or subscribes to notifications

## Deployment

- Infrastructure as Code (AWS SAM or Serverless Framework)
- GitHub Actions for CI/CD
- AWS Always Free Tier eligible

## Scalability

- Auto scaling Lambda functions
- Event driven architecture
- No server management required
- Horizontally scalable system

## Portfolio Value

Demonstrates:

- Event driven microservice design
- Serverless notification architecture
- NoSQL data modeling
- Real time system integration
