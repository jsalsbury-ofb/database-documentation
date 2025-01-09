# Gift Entry

## Batch Review

Open the PDF image files in numberical order, starting with the file that ends with 001. Compare all check image information to the information in Raiser's Edge as displayed in the constituent window in the batch.

### Donor Information

1. Make any updates to addresses, names, designations, appeal and package codes, etc going line by line with the corresponding check images
2. Note any information not already on account- new address, phone number, email, partner name.

### Donor requests

1. Note donor requests for solicitation frequency, branch, memorial, etc in check image file and misc. image file
    1. Make special note of any Tribute requests - mailing a card to the honoree
    2. `Appeal` type, if `GEN`, is changed to `HON` or `MEMORY`
    3. Add honoree’s name to `Honorarium` or `Memorial` attribute description
    4. Link gift to Tribute (use scroll icon at top of batch to find and link)
    5. Make note in [Asana] of donor, recipient, and any specific message included by donor to be sent.
2. Check for ereceipt requests and add to donor profile
    1. Add email address if new - add as type: `Email`
    2. Add `Category`: Special Handling Requirement
        1. **Description**: Electronic communications requested
        2. **Date**: Today’s date
        3. **Comments**: your initials + donor request in `Attributes`

### Gifts greater than or equal to $1000

1. Change `Letter Code` to Standard IND-ORG
2. Check for `Proposal` and link if present
    1. Add `Proposal` name to `Reference` field if applicable

### Individual Retirement Account (IRA) Gifts

Update the gift coding:

| Field                     | Value             |
| ------------------------- | ----------------- |
| `Letter Type`             | IRA Distribution  |
| `Gift Subtype`            | IRA Distribution  |
| `Reference`               | IRA Distribution  |
| `Name on Check`           | *IRA Custodian Name*   |
| `Public Recognition Name` | *IRA Donor Name*  |

!!! info "Note on Reference field"

    In the case where there is a proposal linked to an IRA gift, the "IRA Distribution" takes precedence over the proposal name in the `Reference` field.

??? question "Identifying IRA gifts"

    Gifts from an Individual Retirement Account (IRA) are typically identifiable from the following features: 
    
    **Business check** from a financial institution that manages retirement accounts and investments, such as Vanguard. **Personal check** with IRA or custodian language in the check header, such as "Donor Name IRA" or "Fidelity as Cust." **Distribution letter** attached with check with IRA language, such as "IRA", "QCD." 

## Special Instructions

### End of Year Change-over

The beginning of January it is important to track which gifts have a postmark date of the previous year, for donor tax receipt purposes. Beginning with the first January Lockbox, add the `Postmark Date` column in batch.

??? question "How to add the Postmark Date column"

    Open the `Batch Design` menu and navigate to the third tab `Defaults`. Locate the `Postmark Date Attribute` in the `General` list and unhide it (the default state is hidden). `Save` the updates and return to `Data Entry`.