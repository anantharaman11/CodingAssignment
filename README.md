# CodingAssignment

## Synopsis

Designed a checkout system for mock consumer store using Python

## Installation

	1. Unzip the files and folders
	2. The system designed can be executed in three different ways
		a.	Go to \dist folder and run the Coding_Assignment.exe 
			-	The window prompts for config file path. Check for 'param.ini' file in the unzip location and paste the complete path in the prompts
			-	Review the results
		b.	Execute the Coding_Assignement.py script directly via command prompts
			-	Again, the window prompts for config file path. Check for 'param.ini' file in the unzip location and paste the complete path in the prompts
			-	Review the results
		c.	In worst-case scenario, directly execute the Coding_Assignment.ipynb notebook file in Jupyter IDE or Jupyter Labs.
			-	Again, config file path will be prompted and update the 'param.ini' path in the dialog prompted
			- 	Review the results

	
## Config file interpretation

The param.ini file will be primarily divided into three sections - ProductDetails, PricingRule and ScanInput sections	
-	The PricingRule section will be segregated into - PricingRule1, PricingRule2, PricingRule3, PricingRule4 for each Product ID in the Consumer store

ProductDetails section:
	-	ProductID field: Includes the four Product ID listed in the problem statement, can be varied if needed
	-	Product Name: Includes the four product names listed in the problem statement, can be varied if needed
	-	Price: Includes the four prices of the products listed in the problem statement, can be varied if needed

PricingRule section:
	-	The price discount rule as stated in the problem statement is translated  in the design using these ** six ** fields, where
		a.	Product ID: Product identifier is used as pivotal field to extract purchase and other product information
		b.	Discount type: The type of discounts described in the problem statement is bucketized into four classes such as Price Drop (Sony TV), Free item (Central AC), Buy N Get M (Nike Shoe) and No discount (Charger)
		c.	DiscountThreshold: Indicates the minimum number of item to be purchased to apply discount
		d.	DiscountMetadata: Secondary information in discount formulation and used in Buy N Get M discount category
		e.	DiscountAmount: Amount of discount from the product price
		f.	FreeItem: The free items that will be given due to the discount provided to another product 
		
ScanInput section:
	- ITEM_IDs_Scanned: Typically the scanned input order. Can be tested with varied input combinations.




