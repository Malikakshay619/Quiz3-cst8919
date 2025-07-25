# Quiz 3 - CST8919

## Goal:
Create and assign an Azure Policy that restricts resource deployment to only the Canada Central region.

## Files:
- `only_policy_rule.json`: Contains the policy rule definition.
- `allowed_locations_canadacentral.json`: (Optional) Full policy schema for reference.
- CLI steps documented in bash history.

## Steps performed:
- Created resource group `quiz3` in `canadacentral`
- Created custom Azure Policy with `allowedLocations` parameter
- Assigned the policy to the resource group
- Tested deployment success/failure based on region
