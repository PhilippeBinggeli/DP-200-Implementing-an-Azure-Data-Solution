# DP 200 Implementing a Data Platform Solution Answers
### Lab 1 - Azure for the Data Engineer

## Exercise 1: Identifiy the evolving world of data within AdventureWorks

> Task: From the case study, identify the data requirements of AdventureWorks and identify if the data structure for the requirement is structured, semi-structured or unstructured.

Topic    | Data requirement  | Data structure| Comment |
|-------------|------------- |-------------|-------------|
| AdventureWorks Website | a data store is made available that will hold the images of the products that are sold on the website| Unstructured | Yes, pictures are unstructure data |
| Sales    | global availability, scalability     | Structured  | Yes, this data is structured |
| descriptive analytics    | data warehouse capabilities | structured  | Yes, this data is structured |
| predictive analytics | a recommendation or a text analytics engine | unstructured | No, this data is **semi-structured** |
| Data Warehouse | assessing the tooling that can help with teh extraction, load and transforming (ELT) of data into a DWH | structured | This reque is not mentioned in the solution |
| Customer Services and pre-Sales | support for handling the call volumes through the implementation of chat bots | semi-structured | This reque is not mentioned in the solution |
| Customer Services and pre-Sales | recommendation system | structured | This reque is not mentioned in the solution |
| Customer Services and pre-Sales | check status on current orders | structured | This reque is not mentioned in the solution |
| Customer Services and pre-Sales | find replacement parts | structured | This reque is not mentioned in the solution |
| Customer Services and pre-Sales | discover fraudulent calls | semi-structured | **yes**, this data is consideret to be semi-structured |
| Customer Services and pre-Sales | Chatbot should support global requests | semi-structured | This reque is not mentioned in the solution |
| Customer Services and pre-Sales | Chatbot should support multiple languages | semi-structured | This reque is not mentioned in the solution |
| Social Media Analysis | tracking and measureing the impact of their social media assets | semi-structured | No, this data is considered to be **unstructured** |
| built-in bicycle computer | provide secured information to these computer information | structured | No, this data is **semi-structure**
| built-in bicycle computer | save daily summary data to flat files | structured | Not mentioned in the solution
| bicycle maintenance service | getting notifications on when their bicycle needs repair | semi-structured | **Yes**, this data is considered to be semi-structured

---
## Exercise 2: Determine the Azure Data Platform services to use for AdventureWorks

> Task 1: Determine the data platform technology that delivers the identified data requirements

|Topic | Data requirement  | Technology | Comment |
|-------------|------------- |-------------|-------------|
| AdventureWorks Website | a data store is made available that will hold the images of the products that are sold on the website| Azure BlobStorage | Yes, pictures are unstructure data, Tec is corretct |
| Sales    | global availability, scalability     | SQL Server pool | Yes, this data is structured, no cosmos DB would be better |
| descriptive analytics    | data warehouse capabilities | Azure Cosmos DB  | Yes, this data is structured, no SQL Data Warehouse |
| predictive analytics | a recommendation or a text analytics engine | Azure Cosmos DB | No, this data is **semi-structured**, no Databricks would be the choice |
| Data Warehouse | assessing the tooling that can help with teh extraction, load and transforming (ELT) of data into a DWH | Azure Data Warehouse  (Synaps) | This reque is not mentioned in the solution |
| Social Media Analysis | tracking and measureing the impact of their social media assets | Cosmos DB | No, this data is considered to be **unstructured**, no Steam Analytics / Event Hubs would be better |
| Customer Services and pre-Sales | discover fraudulent calls | Stream Analytics / Event Hubs | **yes**, this data is consideret to be semi-structured |
| built-in bicycle computer | provide secured information to these computer information | structured | No, this data is **semi-structure**
| built-in bicycle computer | save daily summary data to flat files | Stream Analytics / IoT hubs | Not mentioned in the solution, 
| bicycle maintenance service | getting notifications on when their bicycle needs repair | Stream Analytcs / IoT Hubs | **Yes**, this data is considered to be semi-structured

## Exercise 3: Identifiy the tasks to be performed by the data Engineer

Each requirement shoulb be articulated with the following tasks:
- provisioning (Bereitstellung)
- processing
- security
- monitoring
- disaster revcovery

---

### Exercise 4: Finalize the data engineering deliverables for AdventureWorks
> Finalize the data engineering deliverables for AdventureWorks

|Data requirement|Technology|
|---|---|
|A data store is made available that will hold the images of the products that are sold on the website.|Azure Blob|
|Would like to take their data analytics further and start to utilize predictive analytics capabilities.|Databricks|
|A system to better serve customers with global availability of its application and sales and ordering data. |Cosmos DB|
|Data warehouse capabilities of Azure Synapse Analytics|Azure Synapse Analytics|
|The customer services department want to help their agents to identify fraudulent call for support|Stream Analytics / Event Hub|