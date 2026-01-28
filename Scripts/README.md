### Weekly Privileged Snapshot Script (Placeholder)

The file `scripts/Weekly_Privileged_Snapshot_PLACEHOLDER.ps1` is a conceptual placeholder for the automation that would support this control in a real environment.

It documents the expected behavior of the script:

- Connect to Azure Entra ID or Microsoft Graph
- Identify high risk directory roles and admin groups
- Export their memberships to CSV with a timestamp
- Save the file using the ITGC_UAR01 naming convention

In a production environment, this script would be implemented with real Graph calls, authentication, and scheduling, but that logic is intentionally omitted from this public portfolio repo to avoid exposing tenant specific details or secrets.
