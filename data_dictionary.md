# Data Dictionary

Sheet: `Requests`. Columns A to J are inputs. Columns K to T are calculated.

| Col | Field | Description |
|---|---|---|
| A | Request ID | Unique ID (REQ-001 to REQ-060) |
| B | Date Raised | Date the request was received |
| C | Requested By | Person who made the request |
| D | Department | Marketing, Finance, HR, Operations, IT |
| E | Request Type | Presentation, Report, Data Pull, Ad Hoc Analysis, Dashboard Update, To Confirm |
| F | Priority | High, Medium, Low |
| G | Owner | Vikram, Rohan, Sana, Neha, UNASSIGNED |
| H | Due Date | Deadline |
| I | Status | Completed, In Progress, On Hold, Not Started |
| J | Completed Date | Blank if not completed |
| K | Data Check | OK, Duplicate ID, Needs confirmation, or Invalid date |
| L | Days Allowed | Due Date minus Date Raised |
| M | Turnaround Days | Completed Date minus Date Raised (valid records only) |
| N | Delivery | On time or Late (valid completed records only) |
| O | Days Late | Completed Date minus Due Date, if late |
| P | Alert | OVERDUE, DUE SOON (within 3 days) or HIGH OPEN |
| Q | Days Overdue | Report Date minus Due Date for overdue items |
| R | Week Starting | Monday of the week the request was raised |
| S | Next Action | Suggested action for the request |
| T | High-Open ID | Helper used for the dashboard attention box |

## Dashboard input
Report Date (yellow cell, default 19-Nov-2026) decides which open requests are overdue.
