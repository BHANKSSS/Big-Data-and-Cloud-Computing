# Big-Data-and-Cloud-Computing
Wildan Miftakhurahman | 21110040 | S1SD02A

Creating, Importing, Querying, and Exporting Data with Amazon DynamoDB Assignment. 

Objective : In this assignment, you will use the Amazon DynamoDB service to create a table, import data from a CSV file, perform queries or scans with filters, and export the results. Write comprehensive documentation outlining the steps taken to complete this assignment. This documentation should be published on an online platform such as Medium, GitHub, or your personal blog.
## DynamoDB, An Introduction
Amazon DynamoDB is a fully managed NoSQL database service provided by Amazon Web Services (AWS). No-SQL database management solutions are those that depart from the traditional relational database model. For applications seeking speedy and dependable performance, even with a lot of data, it offers low latency, high availability, and seamless scaling. Due to DynamoDB's horizontal scalability, performance stays constant as data and traffic volumes increase by dispersing data across a number of servers. SSDs, which offer read and write operations with single-digit millisecond latency, are utilized for storage.

Thanks to DynamoDB's schema-less data model, fixed table structures and predefined schemas are not required. The way the data is organized, with its tables and items, resembles a key-value store. This versatility enables agile development and easy adaptation to changing data requirements. Additionally, DynamoDB provides automated data replication and multi-region capabilities, ensuring exceptional availability and durability.
## Create a Table in DynamoDB
### 1. First, we search for "DynamoDB" in the AWS service menu.
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/354e29ee-e7e7-41c1-be42-4b93bb10b519)
### 2. Click Table
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/4b923029-5082-4f94-9f96-256f65825863)
### 3. Create Table by click "Create Table"
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/67f24d18-0b7f-4e0c-b1a3-f1ec36fb0e47)
### 4. Table Setting
make sure insert a relevant data type
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/989ab750-4bf2-4f1b-a229-d62113d8814c)
to make it simple, just use the defult setting
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/6b06e3e2-cfa9-4f9f-ac4f-beaf7baf34cb)
no more any customazion? just click "Crate Table"
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/f838c4bb-9434-4dee-9da7-2f13b353caf2)
this is your table, congrataz! finished? no...
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/c87e0169-a743-4678-a2c8-7a877ca37d5e)
wait until the status changet into active
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/ba353a5f-6355-49f9-ae4c-6b8a9ea69769)

### 5. Create Item
click your table name, than just follow this picture, ive no idea how to describe it
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/bf9a2280-b7d1-4b54-a9c8-3562e9edd2b5)
fill the blank
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/d744f55f-e340-430b-87d4-6aa3d565031e)
boom, the item ready to fill with CSV (or other, idk, just got here)
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/6f56c9af-710c-4151-98a7-c5547c3f2ddb)

## Import Data
## 1. Simply select DynamoDB from the menu, click Import from S3, and then select "Import from S3" to import datasets from an S3 bucket.
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/8fc4a89f-e3ce-4c7b-afa9-01a82ed6fa0f)
## 2. to make it easier, upload your CSV into s3 first. so you just need to browse it
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/42b38bde-3532-4a78-b41f-7857b4c34610)
## 3. Choose CSV, or any other format you used. then next
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/2e301701-44ac-475d-988d-f6b083a19c7e)
### 4. now this, crate name and decide primary key for your table
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/6deebcef-dfad-46e1-97f9-7f21372a74b1)
### 5. yes, just default, dont make it harder
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/89506860-1121-4b6a-8ddf-666185b22390)
### 6. import sir
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/f9b8d2f2-2bf6-4c54-8874-b91908d8f321)
### 7. it could take a while
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/66938700-48fc-435e-83f2-b44a61e58dd8)
### 8. it should look like this
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/754276bf-a6d8-4f3a-8406-b6e21bc20a07)
## Scan Data
Scanning and searching for data can help you uncover information more quickly.

Click on Explore Item and scan. just play along with this setting. 
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/efb456e7-d57d-4f02-b707-fb283177e199)
just looking for filled job with less then 50000 input
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/0e4f794d-a65b-47de-b63a-0b7db18883c5)

## Querying Data
In fact, dynamo database queries are very sophisticated, thus for the purposes of this experiment, i look for specific imformation about someone with BDCQ.SED1RP ID
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/64c70611-261e-4304-a0f6-426fe6e9500b)

## Export Data
lets export the result
### 1. you sould already familiar with this
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/3c800191-31f1-4721-9c0b-127d40e9d01e)
addional note. you should turn on the PITR (point-in-time-recovery)  or just follow the recent notificarion

## Conclusion
Amazon DynamoDB is a highly scalable and high-performance NoSQL database service. With a key-value storage model, DynamoDB provides low response times and high throughput. DynamoDB is also flexible in terms of data schemas, allowing arbitrary data storage. With high durability and fault tolerance, DynamoDB maintains high data availability. Overall, DynamoDB is a powerful NoSQL solution for managing large-scale data with fast performance and easy management. With DynamoDB, you can construct tables, import datasets, and run queries or scans to get the information you need.
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/d4749379-484c-4ab0-b196-1192f2056309)
### 2. choose the bucket destination along with wich table you would export
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/bf8265ca-e174-46b0-b644-eb19e5c2fb80)
### 3. surprise, surprice, its already on process
![image](https://github.com/BHANKSSS/Big-Data-and-Cloud-Computing/assets/73731578/627626d3-68dc-46d2-afb4-e9de72d2e0fa)
