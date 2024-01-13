# Retail-Market-Basket-Analysis-and-customer-churn-prediction
The project's goal is to solve the problem that many retail giants like Wallmart, Marks &amp; Spencer, Sobeys, Canadian Tire and et al face. Market analysis through apriori algorithm is performed to find product association and then customer churn prediction is done to provide customers lucaritive incentives that will drive the retail sales.

### About Dataset

The Online Retail dataset encompasses all transactions conducted by a UK-based online retail business registered between December 1, 2009, and December 9, 2011. The company specializes in the sale of distinctive all-occasion gift-ware. Notably, a significant portion of the customer base comprises wholesalers.

<br>Attribute Information:
<br>InvoiceNo: Invoice number. Nominal. A 6-digit integral number uniquely assigned to each transaction. If this code starts with the letter 'c', it indicates a cancellation.
<br>StockCode: Product (item) code. Nominal. A 5-digit integral number uniquely assigned to each distinct product.
<br>Description: Product (item) name. Nominal.
<br>Quantity: The quantities of each product (item) per transaction. Numeric.
<br>InvoiceDate: Invice date and time. Numeric. The day and time when a transaction was generated.
<br>UnitPrice: Unit price. Numeric. Product price per unit in sterling (Â£).
<br>CustomerID: Customer number. Nominal. A 5-digit integral number uniquely assigned to each customer.
<br>Country: Country name. Nominal. The name of the country where a customer resides.

<br>Source:
<br>Dr. Daqing Chen, Course Director: MSc Data Science. chend '@' lsbu.ac.uk, School of Engineering, London South Bank University, London SE1 0AA, UK.

<br>Please find more information refer the below link,
<br>https://archive.ics.uci.edu/ml/datasets/Online+Retail+II

### Data Cleaning
*The granularity of data is based on unique transaction and product combination. 
*The dataset consists of 541909 records.
*The number of duplicate and null records are 5225 and 136534 respectively. The number of records after removing null and duplicates is 400150.
*The purpose for this analysis is to understand customer buying behaviour and based on that we could establish product association rules and targeted marketing strategies.
<br>For this reason it is required to filter out any records that represent product returned or refund from customer.Thus it required to drop records where Quantity<0 and Unit Price <=0. After filtering out such records there was total 392692 records in the dataset.
* Apart from that the product description for few product items was not uniform. The variation in product description is handled by imputation.
* Lastly, the data ranges from 1/12/2010 to 8/12/2011. In order to accurately uncover seasonal trends, the 8 records for month of december 2011 is dropped.
