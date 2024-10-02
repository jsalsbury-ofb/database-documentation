# Merging Records

## Add Merge Attributes

1. Add the **duplicate record's** `Raiser's Edge ID` into the following areas in the original record:
    1. `Bio 1` > `Aliases` > *New Row* > *Merged ID*
    2. `Attributes` > *New Row* > *Merged Record*

!!! danger "Failure to add merge attribtues"

    Failure to add the above attributes during the record merge process will result in exceptions during the import process when importing appeals to records. There is a process to recover some of these missing merged IDs via the appeals master spreadsheet, however please do not neglect this step to ensure data integrity.

## Transfer Bio 1, Bio 2, Address Tabs

1. `Bio 1`
    1. `Aliases`: Copy over all aliases from the duplicate record into the original record.
    2. `Solicit Codes`: Copy over solicit codes from the duplicate record into the original record, and make decisions about which, if any, solicit codes to override or remove from the original record. This is assuming that the duplicate record's codes were added more recently.
    3. `Phones` and `Emails`: Copy over phone numbers and email addresses. Assuming the duplicate record's phone numbers and email addresses were added more recently, you may need to elevate them to the primary contact fields by downgrading the existing ones.
2. `Bio 2`
    1. `Constituent codes`: Add missing constituent codes from the duplicate record into the existing record. This ensures that the original date of the solicit codes of original records in preserved in the merge.
3. `Addresses`: Add any missing addresses from the duplicate record into the original record. Assuming the duplicate record is more up to date, you may elevate the current address to the primary one and downgrade existing addresses on the original record.

## Merge

To complete the merge process:

1. Copy the `Raiser's Edge ID` of the original record, and then close the original record.
2. Open the duplicate record.
3. In the top menu of the duplicate record constituent window, go to *Constituent* > *Merge* > *Merge from (record) into...* > Enter original record ID
    1. The merge window will prompt you to select which tabs from the duplicate record to merge into the original record.
    2. Select all tabs that have a red checkmark, which indicates that a tab has data. **Do NOT select the Bio 1, Bio 2, and Address tabs** in this menu, since those were transfered manually in the previous section.
    3. Proceed with the merge.
4. After the record merge is completed, Raiser's Edge will close out of the duplicate record and open the original record. Verify that the information merged into the record correctly.
5. Close the original record, and re-open the duplicate record.
6. Verify that the duplicate record information was merged. The only tabs that should still have red checkmarks in the duplicate record are Bio 1, Bio 2, and Addresses.
7. Delete the duplicate record by going to *File* > *Delete Constituent*. **Please double check that you are deleting the correct record before completing this step.**
