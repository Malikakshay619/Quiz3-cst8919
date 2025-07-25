# Quiz 3 - CST8919

## Goal:
Create and assign a custom Azure Policy to **deny resource deployment in Canada regions** (canadacentral, canadaeast).

## Steps Performed:
-  Created resource group: `quiz3` in `canadacentral`
-  Wrote a custom policy (`only_policy_rule.json`) to deny deployments in `canadacentral` and `canadaeast`
-  Deleted old parameterized policy and assignment that only allowed `canadacentral`
-  Assigned the new policy at resource group scope using Azure CLI
-  Verified:
  - Deployment in Canada regions fails 
  - Deployment in `eastus` succeeds 

## Files:
- `only_policy_rule.json` – contains the deny rule
- `README.md` – this summary

## Commands used:
- `az policy definition create`
- `az policy assignment create`
- `az storage account create` (for testing)

