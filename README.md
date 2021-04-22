

### profiles to use

- CICD Acct. Admin Privs: cicd-admin
- CICD Acct. DevOps Privs: cicd-devops

- MASTER ACCOUNT ROOT ADMIN: rootbuilder
aws sso login --profile cicd-admin && npx cdk-sso-sync cicd-admin

npm run cdk deploy WebAppPipelineStack -- --profile cicd-admin
