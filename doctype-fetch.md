# 1. Fetching Logic in Doctypes
## Description
 Get the 'warranty' field info from the another doctype (eg: Customer) into the Current doctype (eg:Quotation) based on the Selected Customer('party_name' is the quotation docfield name)
## Basic Syntax
### Fetch from in custom field:
```text
linked_field_name.field_to_fetch
```
## Use Case
Specify the below line of code in corresponding "Warranty" field in Current document
```text
party_name.warranty