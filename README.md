# create-sap-table
Create SQL query to create SAP tables from leanx

Installation  
`pip install create-sap-table`

How to use
```python
from create_sap_table import create_table_leanx

create_table_leanx.get_query('EKKO')
# this should print 'Script generated successfully. File create_EKKO.sql created.'
# and create a new create_EKKO.sql file in the directory

create_table_leanx.get_query('invalid_table_name')
# this should raise an assertion error and print 'AssertionError: No fields returned for the given table name `invalid_table_name`.
# Please check if the table exists on https://www.leanx.eu/en/sap/table/search. If problem persists, please get in touch @n.basaye'
```
