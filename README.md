# Louisville KY Metro Expenditure Data

## About
This data contains Louisville KY Metro Expenditure Data from https://data.louisvilleky.gov, and is provided as a backup data source for a data engineering project. Data is separated by fiscal year (e.g. Fiscal Year 2012 represents July 1, 2011 through July 30, 2012).

## Version
CSVs were downloaded on 4/27/2023 using the previously available reports for each year (with varying 'last updated' dates). If I update this in the future, I'll include the dates these reports were generated.

## License

Open Data PPDL License: https://opendatacommons.org/licenses/pddl/summary/index.html

Info on data source's site:
https://louisville-metro-opendata-lojic.hub.arcgis.com/pages/terms-of-use-and-license

## Data dictionaries
There are two data formats, the data dictionary for each set are defined below (data dictionaries were provided from data.louisvilleky.gov):

### 2008 format (used through 2017):
Field | Description
----- | -----
Fiscal_Year | The fiscal year represents the timeframe in which goods are received or services are performed. Note: A fiscal year starts July 1 and runs through June 30 of the given year. For example, Fiscal Year 2012 would include July 1, 2011 through June 30, 2012.
Budget_Type | Whether the expenditures were due to capital or operational expenses.
Agency_Name | The agency group for which the expenditures belongs.
Sub_Agency_Name | The sub group of the agency group for which the expenditures belongs.
DepartmentName | The department group for which the expenditures belongs.
Sub_DepartmentName | The sub group of the department group for which the expenditures belongs.
Category | A breakdown of what the expenditures were for.
Sub_Category | A further more detailed breakdown of what the expenditures were for.
Stimulus_Type |
Funding_Source | The group which provided the funding.
Vendor_Name | The name of the vendor being paid.
InvoiceID | The invoice ID from the vendor.
InvoiceDt | The date of service as provided on the invoice from the vendor.
InvoiceAmt | The amount invoiced for payment by the vendor.
DistributionAmt | A breakdown of the accounting strings used to pay an invoice. Note: A single invoice amount could be split between more than one distribution.
CheckID | The ID number for the check distributed to the vendor which paid all or part of the invoice.
CheckDt | The date the check was issued to the vendor.
CheckAmt | The amount issued on the check to the vendor. Note: Sometimes a single check can be issued for multiple invoices. The check amount may then be larger than the invoice amount but the invoice amounts from all included invoices will add up to the total check amount.
CheckVoidDt | If applicable, the date a check was voided. Note: 1/1/1900 is the default value. If this is the value the check has not been voided.

### 2018 format (used through 2022):
Field | Description
----- | -----
Fiscal_Year	| fiscal year of the date of payment
Invoice_date	| Date listed on the invoice received
Invoice_Number	| Unique identifier used on the invoice 
Invoice_Amount	| Amount invoiced by the supplier
Payee	| Recipient of payment amount
Payment_Date	| Date of transaction or date check printed
Payment_Number	| Transaction ID or check number
Extended_Amount	| dollar amount paid to payee
Expenditure_Type	| budget type (Operating or Capital)
Fund	| funding source for the expense
Financing_Source	| identifies the funding source (ex. debt funded, forfeiture funds, agency receipts, etc.); a subset of capital expenses
Agency	| agency or department who purchased product or service
Cost Center	| unit within a department the expenses are charged; a subset of the agency
Expenditure_Category	| broad grouping of expenditures
Spend_Category	| subcategory of the broad grouping of expenditures
Project	| optional tag used to identify related expenses
Program	| optional tag used to identify related expenses
Grant	| optional tag used to identify funding from external resources
Region	| council district
