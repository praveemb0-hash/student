# GitHub Upload Guide

1. Extract `SECMS-GitHub-Project.zip`.
2. Open the `SECMS` folder in VS Code.
3. Create an empty GitHub repository named `SECMS` (or another name you prefer).
4. In the project folder run:
```bash
git init
git add .
git commit -m "Initial SECMS Salesforce project"
git branch -M main
git remote add origin <YOUR-GITHUB-REPOSITORY-URL>
git push -u origin main
```
5. Do not commit credentials, tokens, private keys or real student information.
