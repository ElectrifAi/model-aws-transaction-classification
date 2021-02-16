# Input/Output Description

> Note: The client should provide the following formatted data in CSV file (1 required).Below are the details for each CSV file. 

- **_transaction_info.csv_** (*REQUIRED*): 
    
| Column                 | Column Required?  | Meaning                                                     |
|------------------------|-------------------|-------------------------------------------------------------|
| TRANSACTION_ID         | Y                 | Unique transaction ID of the transaction                    |
| SUPPLIER_PARENT_NAME   | Y                 | Supplier name in the invoice of transaction                 |
| SUPPERLIER_NAME        | Y                 | The parent company of the supplier                          |
| MATERIAL_DESCRIPTION   | Y                 | The material/porduct involved in the invoice                |
| GL_ACCOUNT_DESCRIPTION | Y                 | The description of related financial report category        |
| INVOICE_DESCRIPTION    | Y                 | The description in the invoice                              |
| MCC_DESCRIPTION        | Y                 | The description of the supplier's merchandise category code |
| PO_DESCRIPTION         | Y                 | The description of the purchase order                       |
| AMOUNT                 | Y                 | The amount involved in the invoice                          |
 
	
- Output: a JSON list of objects contaning, for each record in the original orderthe following fields:
	- TRANSACTION_ID  : Unique transaction ID of the transaction                      
	- PREDICTION      : Prediction of the transaction type                                                                 
	 
 - Reference file: sample.zip.out	
	
