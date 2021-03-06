# SI_OrderOpener

<img src="oo_pic.PNG"></img>

A GUI application to automate the opening of orders to Lean Supply warehouse. Takes order queries from CommerceHub (Walmart, Best Buy, Staples), CommerceHub CA (The Source), Groupon, and Staples as inputs and combines them into a single output sheet formatted in a way that Lean Supply will accept. Connects to a sqlite database to fetch information on SKU and UPC codes.

## Dependencies:
- Python 3.5
- openpyxl
- sqlite3
- PyQt5

## To-Do:
- ~~Database folder created~~
   - Manage relative path of database
   - Automated updating via webscraping from Harmony 4PL
- Error catching: test for missing UPC, SKU, required shipping columns on main sheet before splitting
- Backorder checks
   - Check sku orders against current inventory
   - Generate report of backorders in each order
   - Running memory of backorders across time (weekly?)
- Add menubar options to update database
- Create db table for Groupon descriptions and associated SKUs, add option to update to menubar
- Update db, fetch excel sheet from Lean Supply


