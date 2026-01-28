# Automation Support Concept: Weekly Privileged Access Snapshots

## Goal

Generate weekly privileged access snapshots from Azure Entra ID to:

- Feed monthly privileged access reviews with fresh data
- Provide time based visibility into who held elevated access during specific weeks
- Support incident response and audit investigations

## Weekly Snapshot Schedule

- Run at the end of each week  
- Store outputs in the evidence binder location for the relevant fiscal year and quarter  
- Use a naming convention consistent with ITGC_UAR01  

Example weekly naming pattern:

`ITGC_UAR01_FY2026_WK02_01_Access_Listing_AzureEntra_Privileged.csv`

## Data to Capture

- User principal name
- Display name (optional)
- Role or group name
- Indicator that the role is privileged
- Export timestamp
- Source system (for example Azure Entra ID)

## High Level Script Workflow

1. Connect to Microsoft Graph or Azure Entra ID.  
2. Identify high risk directory roles and admin groups.  
3. Export memberships into CSV.  
4. Normalize the output into the Access Review Tracker input format.  
5. Save the CSV using the ITGC_UAR01 naming standard.  

## Role In The Control

The weekly snapshots support the control by:

- Providing an up to date listing of privileged accounts for monthly review
- Supporting re performance and investigations by showing who had privileged access in specific time frames

The primary control remains the monthly and quarterly reviews with owner certification. The weekly job is a supporting mechanism that improves completeness and incident response.

