# Gift Entry

## Gifts by Appeal

### 3PW - Third Party Web

<!-- md:version 8/15/2024 -->  <!-- md:flag experimental -->

| Field                     | Value                                                                                 |
| ------------------------- | ------------------------------------------------------------------------------------- |
| `Account Involvement`     | Link Account Involvement (Not the 3PW Vehicle, except ActBlue)                        |
| `Acknowledgement`         | Do Not Acknowledge                                                                    |
| `Appeal`                  | 3PW                                                                                   |
| `Gift Constituent Code`   | Individual                                                                            |
| `Hard Credit`             | Donor, if known. `Anonymous` if not                                                   |
| `Letter Code`             | No Thank You Needed                                                                   |
| `Name on Check`           | 3PW Vehicle (Third-party vendor)                                                      |
| `Reference`               | Donation source                                                                       |

??? question "How to differentiate between 3PW, EMP, and MG?"

    As a reminder, 3PW gifts are gifts that come through a Thirdy-Party Web vehicle, such as ActBlue. EMP and MG gifts can sometimes come through 3PW vehicles, in which case the **Appeal ID** should be updated from 3PW to EMP or MG. Both EMP and MG gifts will have language from the involved company doing the matching. The difference is that EMP gifts will typically have language about "payroll deductions" whereas MG donations will have language about "match" or "matching."

??? question "How to locate 3PW gift breakdown by donor?"

    The exact method will depend on the 3PW vehicle, however there are general steps you can take:
        1. Check for any attached documents with the check distribution. These will often include a link to their web portal where you can view and download the breakdown spreadsheet.
        2. Check the 3PW Raiser's Edge record for any notes or annotations that contains links, and sign in details.
        3. Check the **donorinfo@oregonfoodbank.org** account. Some vendors email the breakdown spreadsheet to this account.

??? example

    Here's an example of how to code a 3PW gift that came through the `Renaissance Giving` vehicle and was attributed to `Josh Salsbury`.

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Account Involvement`     | Renaissance Giving                                                                    |
    | `Acknowledgement`         | Do Not Acknowledge                                                                    |
    | `Appeal`                  | 3PW                                                                                   |
    | `Gift Constituent Code`   | Individual                                                                            |
    | `Hard Credit`             | Josh Salsbury                                                                         |
    | `Letter Code`             | No Thank You Needed                                                                   |
    | `Name on Check`           | Renaissance Giving                                                                    |
    | `Reference`               | Renaissance Giving                                                                    |

### EMP - Employee Giving

=== "Non-local EMP Gift (Most common)"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Account Involvement`     | Link to main business or corporate record                                             |
    | `Acknowledgement`         | Do Not Acknowledge                                                                    |
    | `Appeal`                  | EMP                                                                                   |
    | `Gift Constituent Code`   | Individual                                                                            |
    | `Hard Credit`             | Donor, if known. `Anonymous` if not                                                   |
    | `Letter Code`             | No Thank You Needed                                                                   |
    | `Name on Check`           | Use if different than hard credit donor                                               |
    | `Reference`               | Name of Employee's Company                                                            |

=== "Local EMP Gift"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Account Involvement`     | Link to main business or corporate record                                             |
    | `Acknowledgement`         | Not Acknowledged                                                                      |
    | `Appeal`                  | EMP                                                                                   |
    | `Gift Constituent Code`   | Individual                                                                            |
    | `Hard Credit`             | Donor, if known. `Anonymous` if not                                                   |
    | `Letter Code`             | Non-Receipt TY                                                                        |
    | `Name on Check`           | Use if different than hard credit donor                                               |
    | `Reference`               | Name of Employee's Company                                                            |

??? example

    Here is an example of the correct coding for a **Non-local** EMP gift. Let's say the donor is `Josh Salsbury` making a payroll deduction gift through `Whole Foods`. The appropriate coding is as follows:

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Account Involvement`     | Whole Foods                                                                           |
    | `Acknowledgement`         | Do Not Acknowledge                                                                    |
    | `Appeal`                  | EMP                                                                                   |
    | `Gift Constituent Code`   | Individual                                                                            |
    | `Hard Credit`             | Josh Salsbury                                                                         |
    | `Letter Code`             | No Thank You Needed                                                                   |
    | `Name on Check`           | `Blank` (Assuming the check was issued by Whole Foods)                                |
    | `Reference`               | Whole Foods                                                                           |

### MG - Matching Gift

=== "In Network OR &ge; $250"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Acknowledgement`         | Not Acknowledged                                                                      |
    | `Appeal`                  | MG                                                                                    |
    | `Gift Constituent Code`   | Business / Corporation                                                                |
    | `Hard Credit`             | Business / Corporation matching the gift                                              |
    | `Letter Code`             | Standard IND-ORG                                                                      |
    | `Name on Check`           | Use if different than hard credit donor                                               |
    | `Reference`               | Individual name gift is matching (*Last*, *First*)                                    |

=== "Out of Network AND Under $250"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Acknowledgement`         | Do Not Acknowledge                                                                    |
    | `Appeal`                  | MG                                                                                    |
    | `Gift Constituent Code`   | Business / Corporation                                                                |
    | `Hard Credit`             | Business / Corporation matching the gift                                              |
    | `Letter Code`             | No Thank You Needed                                                                   |
    | `Name on Check`           | Use if different than hard credit donor                                               |
    | `Reference`               | Individual name gift is matching (*Last*, *First*)                                    |

??? example

    Here's an example of an MG gift from `Whole Foods` matching a payroll deduction from `Josh Salsbury`.

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Acknowledgement`         | Not Acknowledged                                                                      |
    | `Appeal`                  | MG                                                                                    |
    | `Gift Constituent Code`   | Business / Corporation                                                                |
    | `Hard Credit`             | Whole Foods                                                                           |
    | `Letter Code`             | No Thank You Needed                                                                   |
    | `Reference`               | *Salsbury, Josh*                                                                      |

### DAF - Donor-Advised Fund

=== "Fund Name Provided"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Acknowledgement`         | Not Acknowledged                                                                      |
    | `Appeal`                  | GEN                                                                                   |
    | `Gift Constituent Code`   | DAF                                                                                   |
    | `Hard Credit`             | Donor, if known                                                                       |
    | `Letter Code`             | Donor-advised Fund                                                                    |
    | `Name on Check`           | Fund Manager's Name                                                                   |
    | `Public Recognition Name` | Fund Name                                                                             |
    | `Reference`               | Fund Name                                                                             |

=== "Fund Name Not Provided"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Acknowledgement`         | Not Acknowledged                                                                      |
    | `Appeal`                  | GEN                                                                                   |
    | `Gift Constituent Code`   | DAF                                                                                   |
    | `Hard Credit`             | Donor, if known                                                                       |
    | `Letter Code`             | Donor-advised Fund                                                                    |
    | `Name on Check`           | Fund Manager's Name                                                                   |
    | `Reference`               | *a donor-advised fund*                                                                |

=== "Anonymous Donor"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Acknowledgement`         | Do Not Acknowledge                                                                    |
    | `Appeal`                  | GEN                                                                                   |
    | `Gift Constituent Code`   | DAF                                                                                   |
    | `Hard Credit`             | Anonymous                                                                             |
    | `Letter Code`             | No Thank You Needed                                                                   |
    | `Name on Check`           | Fund Manager's Name                                                                   |
    | `Public Recognition Name` | Fund name, if known                                                                   |
    | `Reference`               | Fund name, if known                                                                   |

??? info "Oregon Community Foundation (OCF) and Oregon Jewish Community Foundation (OJCF) Exceptions"

    Soft credit the donation back to OCF or OJCF record.

??? info "Oregon Lawyers Against Hunger (OLAH) Exception"

    This is an uncommon occurence. If you receive a gift like this, use the team name in the `Gift Reference` and let DRC know in batch notes to replace the team name with "DAF."

### IFFD - Independent Food and Funds Drive

| Field                     | Value                                                                                 |
| ------------------------- | ------------------------------------------------------------------------------------- |
| `Account Involvement`     | For large IFFDs, link to main CORP or IND record sponsoring the activity              |
| `Acknowledgement`         | Not Acknowledged                                                                      |
| `Appeal`                  | IFFD                                                                                  |
| `Letter Code`             | 3-Part Letter                                                                         |
| `Reference`               | IFFD Name                                                                             |

??? warning "IFFD Gift Reference Naming Conventions"

    The letter will put the IFFD name into this sentence: "*...through your participation in a food and funds drive sponsored by {name of IFFD}...*" **DO NOT** include "Fund Drive"  in the IFFD name such as Bards Turkey Dinner Fund Drive, rather, Bards Turkey Dinner, or Intel or US Bank etc. **If linked to a proposal, do not add proposal name in reference**.

### Box (West or 33rd)

=== "OFB 33rd Office"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Acknowledgement`         | Do Not Acknowledge                                                                    |
    | `Appeal`                  | BOX                                                                                   |
    | `Hard Credit`             | Anonymous                                                                             |
    | `Letter Code`             | No Thank You Needed                                                                   |
    | `Package`                 | Cash                                                                                  |

=== "OFB West Office"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Acknowledgement`         | Do Not Acknowledge                                                                    |
    | `Appeal`                  | BOX                                                                                   |
    | `Hard Credit`             | Anonymous                                                                             |
    | `Letter Code`             | No Thank You Needed                                                                   |
    | `Package`                 | Cash                                                                                  |
    | `OFB Branch Attribute`    | OFB West                                                                              |

### CR-Local / CR-FA - Cause Related Marketing

=== "CR-Local"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Account Involvement`     | Only if different from main CORP record                                               |
    | `Acknowledgement`         | Not Acknowledged                                                                      |
    | `Appeal`                  | CR-Local                                                                              |
    | `Package`                 | IND or ORG                                                                            |
    | `Gift Constituent Code`   | BUS or ORG                                                                            |
    | `Hard Credit`             | Organization or Business                                                              |
    | `Letter Code`             | Standard IND-ORG                                                                      |
    | `Name on Check`           | Name of entity on check                                                               |
    | `Reference`               | Proposal, if applicable                                                               |

=== "CR-FA"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Account Involvement`     | Only if different from main CORP record                                               |
    | `Acknowledgement`         | Not Acknowledged                                                                      |
    | `Appeal`                  | CR-FA                                                                                 |
    | `Package`                 | *None*                                                                                |
    | `Gift Constituent Code`   | BUS or ORG                                                                            |
    | `Hard Credit`             | Organization or Business                                                              |
    | `Letter Code`             | Standard IND-ORG                                                                      |
    | `Name on Check`           | Name of entity on check                                                               |
    | `Reference`               | Proposal, if applicable                                                               |

??? tip "Difference between IND and ORG package"

    **Use the IND package when the money is coming from the individual donors.** For example, if a grocery store is doing a round-up for OFB at checkout program, that should receive the IND package because the round-up money is coming from the individual customers - the grocery store is simply the one who is collecting and sending the money to us. On the other hand, **use the ORG package when the money is coming from the organization's proceeds**. For example, if a furniture store does a campaign where $10 of every chair sold goes to OFB, that should receive the ORG package because the donated funds are coming from the organization's revenue.

### Bequest

| Field                     | Value                                                                                 |
| ------------------------- | ------------------------------------------------------------------------------------- |
| `Acknowledgement`         | Not Acknowledged                                                                      |
| `Appeal`                  | GEN                                                                                   |
| `Campaign`                | BEQUEST                                                                               |
| `Fund`                    | GENOPS                                                                                |
| `Letter Code`             | Standard IND-ORG                                                                      |
| `Reference`               | *"Bequest from Estate of ..."*                                                        |

!!! tip "Notify DRC About Bequests"

    Please include any bequest gifts in batch notes.

### GFD - Great Food Drive with KGW

| Field                     | Value                                                                                 |
| ------------------------- | ------------------------------------------------------------------------------------- |
| `Acknowledgement`         | Not Acknowledged                                                                      |
| `Appeal`                  | GFD 20XX                                                                              |
| `Campaign`                | BEQUEST                                                                               |
| `Fund`                    | GENOPS                                                                                |
| `Letter Code`             | Standard IND-ORG                                                                      |
| `Reference`               | *"Bequest from Estate of ..."*                                                        |

### K12 - School Drives

| Field                     | Value                                                                                 |
| ------------------------- | ------------------------------------------------------------------------------------- |
| `Account Involvement`     | *Link to school record*                                                               |
| `Appeal`                  | K12                                                                                   |
| `Letter Code`             | 3-Part Letter                                                                         |
| `Reference`               | *"School name"*                                                                       |

### GALA

### OHD - Oregon Harvest Dinner

=== "Default

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Acknowledgement`         | Not Acknowledged                                                                      |
    | `Appeal`                  | OHD 20XX                                                                              |
    | `Campaign`                | EVENT                                                                                 |
    | `GL Post Date`            | *First day of event*                                                                  |
    | `Letter Code`             | OHD Letter                                                                            |
    | `Package`                 | Tickets, Sponsorship, or Donation                                                     |

=== "Donor-advised Fund"

    | Field                     | Value                                                                                 |
    | ------------------------- | ------------------------------------------------------------------------------------- |
    | `Acknowledgement`         | Not Acknowledged                                                                      |
    | `Appeal`                  | OHD 20XX                                                                              |
    | `Campaign`                | EVENT                                                                                 |
    | `GL Post Date`            | *First day of event*                                                                  |
    | `Letter Code`             | OHD Letter                                                                            |
    | `Package`                 | Tickets, Sponsorship, or Donation                                                     | 
    | `Reference`               | *DAF name*                                                                            | 

### VOL - Volunteer Activities

| Field                     | Value                                                                                 |
| ------------------------- | ------------------------------------------------------------------------------------- |
| `Appeal`                  | VOL                                                                                   |
| `Package`                 | Shift                                                                                 |

### Endowment

| Field                     | Value                                                                                 |
| ------------------------- | ------------------------------------------------------------------------------------- |
| `Appeal`                  | GEN                                                                                   |
| `Campaign`                | ENDOW                                                                                 |
| `Fund`                    | ENDOW                                                                                 |
| `Letter Code`             | Standard IND-ORG                                                                      |
