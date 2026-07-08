# TenantHub AWS Deployment

## Architecture

(image)

## AWS Services Used

- ECS Fargate
- ALB
- API Gateway
- DynamoDB
- SSM Parameter Store
- IAM
- ECR
- CloudWatch
- S3

## Deployment Flow

1. Docker image built
2. Image pushed to ECR
3. ECS task deployed
4. ALB configured
5. API Gateway proxy created
6. DynamoDB connected
7. Paystack integrated

## Validation

### ECS

(screenshot)

### Health Check

(output)

### Tenant API

(output)

### Payment Verification

(output)

### Database Update

(output)

## Lessons Learned

- ECS secret injection using SSM
- VPC endpoint networking
- API Gateway proxy integration
- IAM least privilege
