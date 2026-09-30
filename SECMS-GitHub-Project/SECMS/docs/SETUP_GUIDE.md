# Setup Guide

## 1. Install prerequisites
Install Salesforce CLI (`sf`) and VS Code with Salesforce Extension Pack.

## 2. Authenticate
```bash
sf org login web --alias secms-dev
```

## 3. Deploy metadata
```bash
sf project deploy start --source-dir force-app --target-org secms-dev
```

## 4. Open org
```bash
sf org open --target-org secms-dev
```

## 5. Assign permission sets
Use Setup > Permission Sets and assign the SECMS permission set matching the user's role.

## 6. Configure org-dependent items
Configure the Training Manager approver, activate required flows after reviewing them, and complete any report/dashboard adjustments required by the target org.

## 7. Load data
Use Data Import Wizard or an appropriate Salesforce CLI data import method. Resolve lookup relationships by Salesforce IDs in the target org; the sample CSV uses human-readable names for clarity.
