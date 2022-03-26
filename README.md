# deklarera-krypto
Automates declaration of crypto assets for Swedish citizens. Creates a K4 report for Skatteverket.

## Prerequisites
* all your transactions have been made through coinbase
* you have only bought, sent, and converted crypto (mining, staking etc. is not supported)

## Get started
* download this repository
* go to https://www.coinbase.com/reports and download the csv file of all your transactions. store it as `transactions.csv` in the data folder.
* enter you personal details in `data/personal_details.json`. Make sure the file is in UTF-8 format (the script will check this).
* run the script, a K4 report will be created if everything works.

## How it works
* the K4 report from Skatteverket is downloaded for the year specified.
* `data/personal_details.json` is checked for errors and then entered in the report.
* `data/transactions.csv` is checked for errors and then the transactions for the year specified are entered in the report.

## Example runs
` ./declare.py 2021 `
