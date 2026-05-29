# Data Dictionary

This file explains the fields used in the incident dataset for the Strategic IT Operations Dashboard.

| Field | Description |
|---|---|
| Ticket ID | Unique identifier for each incident ticket. |
| Priority | Incident priority level, such as P1, P2, P3, or P4. |
| Support Team | Team assigned to resolve the incident. |
| Opened Date | Date when the incident was opened. |
| Resolved Date | Date when the incident was resolved. |
| SLA Target Hours | Maximum allowed resolution time according to the SLA. |
| Actual Resolution Hours | Actual number of hours required to resolve the incident. |
| Breached SLA | Indicates whether the ticket breached the SLA: Yes or No. |
| Breach Reason | Main reason associated with the SLA breach. If there was no breach, this can be N/A. |

## Suggested Tableau Calculated Fields

| Calculated Field | Logic |
|---|---|
| Total Tickets | Count of Ticket ID |
| SLA Breaches | Count of tickets where Breached SLA = Yes |
| Breach Rate | SLA Breaches / Total Tickets |
| Resolution Variance | Actual Resolution Hours - SLA Target Hours |
| SLA Status | Met if Breached SLA = No; Breached if Breached SLA = Yes |
