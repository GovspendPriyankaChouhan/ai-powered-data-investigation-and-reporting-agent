# Privacy and Security

## Overview

This repository is designed as a portfolio project demonstrating an AI-powered data investigation and reporting workflow.

The public repository does not include production credentials, passwords, API keys, confidential database records, or sensitive business information.

## Credential Management

Credentials used by the workflow should be stored securely within the relevant platform or credential management system.

Examples include:

- PostgreSQL credentials
- Google credentials
- AI model API credentials
- Email service credentials

Sensitive credentials should never be committed directly to a public GitHub repository.

## Database Access

The workflow uses PostgreSQL for database investigation and SQL-based data operations.

In a production implementation, database access should follow the principle of least privilege. Service accounts should only receive the permissions required for their specific tasks.

## AI Processing

AI agents are used for:

- Database investigation
- Data cleaning support
- Executive report generation

Before implementing similar workflows with production data, organizations should review what information is being sent to external AI services and ensure that the appropriate privacy and data governance requirements are met.

## Human Review

The workflow includes an approval process before data cleaning actions proceed.

This human-in-the-loop design helps provide additional control over automated data operations.

## Repository Safety

This public repository is intended to demonstrate the project architecture and workflow design.

It does not intentionally expose:

- API keys
- Passwords
- Database connection strings
- Confidential customer information
- Production database data
- Proprietary business information

## Recommendation

For production environments, additional security measures should include:

- Role-based access control
- Environment-specific credentials
- Secure secret management
- Database activity logging
- Input validation
- SQL access restrictions
- Monitoring and audit trails
