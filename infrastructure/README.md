# Infrastructure Assets

This directory contains AWS infrastructure configuration files created during the TenantHub deployment.

## IAM

- `ecs-trust-policy.json` – Trust policy for ECS task roles.
- `codebuild-trust.json` – Trust policy for the CodeBuild service role.
- `github-actions-oidc-trust.json` *(optional)* – Trust policy used for GitHub Actions OIDC authentication.

## CodeBuild

- `buildspec.yml` – Example build specification.
- `codebuild-project.json` – CodeBuild project definition.

## Note

During the project, an initial CI/CD design using AWS CodeBuild was prepared. Due to AWS account verification restrictions, the production deployment pipeline was implemented using **GitHub Actions**, which built and pushed Docker images to Amazon ECR before deployment to Amazon ECS Fargate.

These files are retained for reference and to document the project's evolution.
