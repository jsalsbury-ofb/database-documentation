# Deceased Constituents

## Deceased is the Primary Record

1. If the deceased constituent is the primary record holder, check if they have a **Partner**.
    1. If the primary record holder has a **Partner** on record, you need to manually flip the records such that the primary record holder becomes the new partner record, and the partner record becomes the new primary record holder.
    2. From here, please proceed to the next section and follow the steps for deceased relationshiop record.
2. Update the `Bio 1` tab.
    1. Add **Solicit Code** `No Mail at All - Per OFB` on the `Bio 1` tab.
    2. Check the **No Valid Address** box on the `Bio 1` tab.
    3. Check the **Deceased** box and add the deceased date, if known.
3. Update the `Addresses` tab.
    1. Go through any active addresses on record, and uncheck the **Send mail** box.
4. Add an `Action` on the **Actions** tab.
    1. Select the **New Action** button.
    2. Use the `Shift + F2` shorcut to load the default action.
    3. Go to the **Notes** tab and create a new note titled `{Constituent Name} deceased`.
    4. Add any relevant notes about why the constituent is being marked as deceased, including: remit notes, Nexis research, relative phone call, obituary, etc.

## Deceased is a Relationship Record

1. Open the relationship record.
2. Update the `Bio 1` tab.
    1. Add a `Date To` (end date) for the relationship using the current date.
3. Update the `Bio 2` tab.
    1. Check the **Deceased** box and add the deceased date, if known.

!!! info "If the relationship record type is Partner"

    If the relationship is specifically `Partner`, update the relationship type `Deceased Partner` - `Widow / Widower`. If it is specifically a spousal relationship, update the primary record holder `Bio 1` tab **Married Status** to `Widowed`.

## Deceased Finder

## Bequests

### What is a Bequest?

A bequest is a gift that a donor has directed be given to an organization upon their death, usually as part of a will. Bequests can either be planned or unsolicited, and can be designated to a specific fund if the donor indicated such. Bequests often are sent via the deceased donor's executor, attorney, or financial agent but should be considered a gift from the estate of the deceased donor.

!!! info "Note about Endowments"

    Bequests should not be designated to the Endowment unless specifically directed by Development leadership.

### Updating Constituent Record

1. If the donor is deceased but their record has not been updated to reflect this, follow the standard procedures for marking a constituent deceased, outlined above.
2. Update the **preferred addressee** to `Estate of {Donor Name}` and **salutation** to `{Name of Executor}`.
    1. Example:
        1. *Addressee*: Estate of Joan Crawford
        2. *Salutation*: John Smith (executor)
3. If the contact address of the estate executor is different from the donor's, add the executor as a new **preferred address** and save the donor's address as a **Prior Address**.
    1. A best practice is to add the name of the executor/fiscal agent in the address line using the `c/o` notation. For example:

```
Estate of Joan Crawford (addressee will merge in letter)
c/o John Smith, Attorney at Law
12345 Hollywood Blvd
Los Angeles, CA 90214-1234
```
