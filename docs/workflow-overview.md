# Workflow Overview

## Purpose

This workflow demonstrates an AI-powered approach to investigating database issues, supporting data cleaning, and generating executive-level reports.

The process is orchestrated in n8n and combines AI agents with SQL queries, workflow logic, human review, and Google Workspace tools.

## Workflow Stages

### 1. Investigate the Database

The workflow starts with the **Data Investigator** AI agent.

The agent analyzes database information and uses PostgreSQL SQL queries to investigate potential issues.

The output is structured so that it can be processed consistently by the rest of the workflow.

### 2. Review and Approval

Investigation results are filtered and routed through an approval process.

Gmail is used to communicate investigation findings and collect responses.

Conditional logic determines whether an issue should proceed to the data cleaning stage.

### 3. Clean and Resolve Issues

Approved items are processed individually.

The **Data Cleaner** AI agent supports the issue-resolution process using:

- Google Gemini
- PostgreSQL SQL queries
- Structured outputs
- Additional n8n sub-workflows

This stage demonstrates how AI-assisted analysis can work alongside SQL-based data operations.

### 4. Generate an Executive Report

The results from the investigation and cleaning stages are merged and aggregated.

The **Report Generator** AI agent creates an executive-level summary.

The final report is then:

1. Created in Google Docs
2. Updated with the generated content
3. Shared through Google Drive
4. Communicated through Gmail

## Workflow Outcome

The workflow transforms a data issue investigation into a structured end-to-end process:

```text
Identify Issues
      ↓
Investigate Database
      ↓
Review and Approve
      ↓
Clean and Resolve
      ↓
Aggregate Results
      ↓
Generate Executive Report
      ↓
Share and Notify
