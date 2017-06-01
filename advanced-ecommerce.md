## eCommerce Tracker

Your eCommerce business needs to keep track of products and their prices. The products each belong to a department. The business needs to keep track of revenue as product prices change over time. The business also needs to keep track of receipts of transactions and the number of units each product has in stock.

Departments > Products with Prices
Transactions
Product Prices & Inventory

Department Document:
* departmentName: String
    * Must be at least 4 characters
* products: subdocument nested index list

Products Subdocument:
* productID: Integer
    * Must be at least 1 character
* productName: String
    * Must be at least 3 characters
* productPrice: Number
    * Must have 2 decimal numbers e.g. XX.00
* productStock: Integer
    * Cannot be less than 0

Transactions Document:
* transactionID: Integer
    * Must be at least 1 character
* productIDs: Array
    * Cannot be empty

Can be used for revenue analysis and inventory analysis:
Products Document:
* productID: Integer
    * Must be at least 1 character
* productName: String
    * Must be at least 3 characters
* productPrice: Number
    * Must have 2 decimal numbers e.g. XX.00
* productStock: Integer
    * Cannot be less than 0