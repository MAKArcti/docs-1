---
description: After the Epoch completes
---

# Paying Your Team

#### At the end of an epoch, export a CSV of the epoch data for analysis and distribution.

![Admin Epoch History](<../../../.gitbook/assets/image (32).png>)

Currently, the only way to pay your team is to download the CSV and use it to pay your contributors.

Since this is a CSV, you can use this file to pay your team however you'd like and on any chain you'd like; know that the addresses your contributors used to sign in are the ETH mainnet addresses.

### CSV Templates

[Coordinape USDC + GOV Token Rate Template](https://docs.google.com/spreadsheets/d/1qXdhFvtYkuiJE1MHOkwx0WuVWlbKgwfDjZeDrb6JAC4/edit?usp=sharing)

### Payment Disbursement

If you're paying your team on Ethereum, you can use any of the apps below, pay them in individual transactions, or a custom script.

<details>

<summary>Disperse</summary>

In the [Disperse ](broken-reference/)app after you have your csv you can distribute the tokens you wish to allocate by pasting the token address into the token address section

<img src="../../../.gitbook/assets/image (18).png" alt="" data-size="original">

Then you'll need to take the address and the amount and paste it into the box below.

<img src="../../../.gitbook/assets/image (27).png" alt="" data-size="original">

When you're done, make sure it looks ok and then, click approve and then disperse token

<img src="../../../.gitbook/assets/image (13).png" alt="" data-size="original">

</details>

<details>

<summary>Gnosis Safe</summary>

* Log into your safe

<!---->

* Click apps, search Csv, and select CSV Airdrop
  1. ![](<../../../.gitbook/assets/image (12).png>)

<!---->

*   Format your Coordinape csv correctly:

    Preparing a Transfer File

    Transfer files are expected to be in CSV format with the following required columns:

    * **`token_type`**: The type of token that is being transferred. One of `erc20,nft` or `native`. NFT Tokens can be either ERC721 or ERC1155.
    * **`token_address`**: Ethereum address of ERC20 token to be transferred. This has to be left blank for native (ETH) transfers.
    * **`receiver`**: Ethereum address of transfer receiver.
    * **`amount`**: the amount of token to be transferred. This can be left blank for erc721 transfers.
    * **`id`**: The id of the collectible token (erc721 or erc1155) to transfer. This can be left blank for native and erc20 transfers.

    **Important: The CSV file has to use "," as a separator and the header row always has to be provided as the first row and include the described column names.**

<!---->

* Upload your csv and click submit.
  1. ![](<../../../.gitbook/assets/image (30).png>)

</details>

<details>

<summary>Utopia Labs</summary>

[Loom Video](https://www.loom.com/share/38d2eb121d044c759555dfdf61c271fa)

### Step by Step Tutorial

#### Before Uploading

1. Download the raw data from Coordinape, and upload that into this Google Sheets template [here.](https://docs.google.com/spreadsheets/d/1z4nDeBKj9Z81se3YIsiaY8JpbnVgz4vI78mUzeRgW6g/edit?usp=sharing)
2. Remove all of the contributors that received 0 GIVE.
3. Remove the “sent” column, which is the column that outlines how much contributors gave to others.
4. Sum up the received column at the bottom
5. Add a column that says “% of budget”
   1. Divide the amount received per contributor by the total sum to get the % of the budget that they’re going to receive.
   2. Add the total budget amount that you planned to pay for this circle/epoch at the bottom of the % of budget column.
6. Add another column that says total received based in USD
   1. Multiply the % of the budget by the total budget amount
   2. By doing this, you know the breakdown of how much the contributor should get paid.

#### If the user gets paid in one token, you can move forward with adding two more columns

1. **Amount denominated in \_(optional) We currently support 5 currencies: USD, CAD, EUR, GBP, AUD**\_
   1. This should only be for native token amounts. If you’re paying out in USDC, leave this form field blank.
2.  **Pay-out Token (Required)**

    1. The token you’re paying out in.

    [CSV Payments](https://www.notion.so/a361f457363a4a8fb8eb7a59bd5aaf93)
3. Upload the CSV in Utopia

#### IF the contributor gets paid in MULTIPLE tokens, then you’re going go to have to do the following:

1. Create 3 more columns for each token:
   1. Amount
   2. **Amount denominated in** _(optional) We currently support 5 currencies: USD, CAD, EUR, GBP, AUD_
   3. Pay-out Token
   4. Calculate the amounts accordingly.
      1. If you’re paying out in two tokens (assuming you’re paying an equal allocation of each token, divide the total received based in USD by 2
2. Create a new sheets, and copy paste the first table with only the first section of the first token into another sheet.
3. Then, paste the second token amounts UNDERNEATH the first token amount table.
   1. This means that you’re going to have duplicate contributors, wallets, etc.
   2. Again, paste as values only.
   3. In this case tho, if you’re paying out in native tokens, and denominating it based in USD, you would have to add “USD” in the “**Amount denominated in** _(optional) We currently support 5 currencies: USD, CAD, EUR, GBP, AUD” column._

Therefore, if you’re paying out an individual with multiple tokens, then each token requires a new row, meaning duplicate individuals.

Once you have this available, you’re ready to import into Utopia!

</details>

<details>

<summary>Parcel</summary>

Coming Soon! 👀

</details>
