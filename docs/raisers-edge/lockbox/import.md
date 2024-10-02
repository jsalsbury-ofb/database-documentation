# Getting Started

## Assigning yourself to the batch on Asana

On [Asana], navigate to the **Donations Processing** project. Either create a `Task` using the `Lockbox Bundle` template, or assign yourself to the existing task under **Project Creation**. When you are ready to begin, please move the task to **Batch Input**.

[Asana]: https://app.asana.com/0/1202332953464341/1205116146297951

## Import Process

Identify the `Lockbox` file for import. This can be found at:

=== "Local"

    ```
    S:\Development\Applications\US Bank Lockbox\Downloads\US Bank Data Files
    ```

=== "VPN"

    ```
    \\Client\S$\Development\Applications\US Bank Lockbox\Downloads\US Bank Data Files
    ```

## Update Defaults

Create or update the relevant `Raiser's Edge` defaults listed below with the **Lockbox Date**. Note, you can use the `F3` shortcut to populate a date field with the current date, if the current date matches the `Lockbox` date.

1.  Individuals: **Initials - New Individual**
    1. Address and Phones
        1. Date From: Lockbox Date
    2. Constituency Codes
        1. Date From: Lockbox Date
2.  Organizations: **Initials - New Organization**
    1. Address and Phones
        1. Date From: Lockbox Date
    2. Constituency Codes
        1. Date From: Lockbox Date
3. Gifts
    1. General
        1. Date: Lockbox Date
        2. GL Post Date: Lockbox Date
4. Individual Relationship: **Initials - Partner**
    1. General
        1. Date From: Lockbox Date
    2. Address and Phones
        1. Date From: Lockbox Date
5. Organization Relationship: **Initials - New Org Contact**
    1. General
        1. Date From: Lockbox Date
    2. Address and Phones
        1. Date From: Lockbox Date

## Import Lockbox Data File Using `Import-o-matic`

1. Open `Import-o-matic` from your `Raiser's Edge` Home Page.
2. Select the `Configure` option from the `Import-o-matic` home and select your `Lockbox` import profile.
3. Navigate to the **Gifts** panel and update the `Description` field to `MM/DD/YY - Lockbox Gifts`.
4. Select your `Lockbox` Import Profile and the file to be imported.
5. Hit the `Import` button and review any potential matches, search for existing records, and addresses to update.

## Batch Setup

1. Open the imported batch.
2. Update the batch description to `MM/DD/YY - Lockbox Gifts`
3. Update the `Projected number of gifts` and the `Projected amount` based on the totals from the import file.

??? question "How do I locate the Gift Batch Setup menu?"

    Once you have opened the batch, navigate to the menu of icons at the top header of the window. Select the `Batch Design` protractor icon to open the Gift Batch Setup menu. Enter any changes, and then hit the Save button.

## Download Image Files from US Bank Lockbox

1. Go to the [US Bank Lockbox] portal and sign in using your credentials.
2. Navigate to **Batch Recap**
3. Enter the desired Lockbox date as the **Start Date** and **End Date**
4. Download all batches to Images files in the Lockbox folder as a dated file folder.

??? question "Setting up an account with US Bank Lockbox credentials"

    Please see the one of the prior sections **Lockbox** for more information.

[US Bank Lockbox]: https://singlepoint.usbank.com/cs70_banking/logon/sbuser