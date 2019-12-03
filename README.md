# Data Privacy Information from CSV file

Turnkey html/js that displays data privacy information from vendors using a simple csv file.

### Requirements
- Jquery (import included)
- Bootstrap (imports included)
- Font awesome (import included)
- Correctly formatted csv file with the following fields (see example file 'DataPrivacy.csv'):
Vendor Name, Product Name, Policy Link, Login Method, Library can see PII, Data kept by vendor, Last Updated

Note: Do not change column names in csv file without also editing the field name in the html file.

### Usage
You will need your csv file to be reachable via a url on your server eg: https://www.mysite.com/files/MyDataPrivacyTable.csv

Edit the following line in data_privacy_csv_file.html to point to your csv file:
```
$.get('/files/data_privacy/DataPrivacy.csv', function(data) {
```
Point your browser to the html file, eg:
https://www.mysite.com/files/data_privacy_csv_file.html
