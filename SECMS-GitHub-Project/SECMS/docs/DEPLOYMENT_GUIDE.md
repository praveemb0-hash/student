# Deployment Guide

## Portable metadata
Custom objects, fields, validation rules, record types, layouts, tabs, application metadata, permission sets and documentation are included in source format.

## Org-specific configuration
The approval approver/user and some report/dashboard runtime configuration can be org-specific. Configure these in Setup after deployment.

## Validation
```bash
sf project deploy preview --source-dir force-app --target-org secms-dev
```
Then deploy:
```bash
sf project deploy start --source-dir force-app --target-org secms-dev
```

Actual deployment success must be verified against the target Salesforce API version and org configuration.
