CyberSource provides a daily XML file with the transactions from the previous day. One customer's daily file contains about 20GB of XML. Each record has about 100 fields. We normalize about half of them into database columns in a relational database, and skip the fields that don't seem to matter to our application.

Today the customer asked why the "EIC" field isn't available in the UI. This is one of the fields we don't load.




dom objects in memory
crashing mid-stream
fields we don't understand
format / field changes from customer to customer
auth/settle linking
monitoring
