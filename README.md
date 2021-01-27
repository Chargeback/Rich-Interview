CyberSource provides a daily XML file with the transactions from the previous day. One customer's daily file contains about 20GB of XML. Each record has about 100 fields. We normalize about half of them into database columns in a relational database, and skip the fields that don't seem to matter to our application.

Today the customer asked why the "EIC" field isn't available in the UI. This is one of the fields we don't load.

Q1. Assuming we add the column to the database, what will we have to do to backfill data from the files?

A new customer signed up today, and their XML feed shares about 90 fields with other customers, but has different names for 5 fields, and has 5 fields other customers don't have.

Q2. How can we modify our file parser to account for these field differences.

Q3. Should we think about storing the data in a different format?

Today the customer mentioned that only about half the file loaded.

Q4. How can we ensure the entire file loads, even if something crashes partway through?

Customers have been complaining that, even though we download the file around 7:00 a.m., and it does load all the way, sometimes not all the records are available until the afternoon.

Q5. What can we do to make the file load more quickly?


dom objects in memory
crashing mid-stream
fields we don't understand
format / field changes from customer to customer
auth/settle linking
monitoring
