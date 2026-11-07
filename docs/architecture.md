# System Architecture

## Overview

The AI-Powered Data Investigation and Reporting Agent is an n8n-based workflow designed to investigate database issues, support data cleaning through SQL, and automatically generate an executive-level report.

The workflow combines AI agents, PostgreSQL, Google Gemini, Gmail, Google Docs, and Google Drive to move from issue identification through investigation, review, remediation, and reporting.

## Architecture Flow

The solution is organized into four main stages:

1. **Database Investigation**
2. **Initial Approval and Review**
3. **Data Cleaning and Issue Resolution**
4. **Executive Report Generation**

## High-Level Workflow

```text
Database Investigation
        ↓
Data Investigator AI Agent
        ↓
SQL Investigation
        ↓
Initial Approval Process
        ↓
Data Cleaning
        ↓
SQL-Based Issue Resolution
        ↓
Executive Report Generation
        ↓
Google Docs and Google Drive
        ↓
Email Notification
