## Ride Share Analytics

Implemented Database Architecture for Uber APP, to keep track of its massive database of drivers, riders and the data generated from each trip. The end-to-end lifecycle of designing a database, sourcing, extracting, and loading data, is implemented. The modelled database is then queried by writing views, stored procedures, ad-hoc select queries, and functions to derive useful insights to expand business.

## Database Design:

The database is designed using star schema, a fact table which hold the measurable, quantitative data about the trips, and dimension table which are 
descriptive attributes related to fact data. The database consists of total nine tables.

- DriverDim
- CabDim 
- RiderDim
- LocationDim
- RiderPaymentInfoDim
- PaymentSchheduleLookup
- IncentiveProgramLookup
- CouponDim
- TripFact

## Steps Involved:

- Conceptual design  - figured out entities and the relationship, rrom all dimension tables to fact table the relationship is 1 to many(1:M)
- Logical Design     - defined attributes, primary and foreign keys for all the tables
- Physical design    - defined data types for all the attributes 
- Big query was choosen because it is serverless, auto scalable and no capacity planning overheads
- Created a project in bigquery, with editor access using IAM roles
- All the dimension and fact tables were created using Create statement(s) and the data was inserted using insert statement(s).
- Encrypted the PII data(card_number) of customer in RiderPaymentInfoDim dimension table and evaluate the data was encrypted.
- Views, stored procedures, ad-hoc select queries, and functions were implemented to analyse and draw useful insights.

## Summary

The Physical design of the Uber App database architechture is shown in the below diagram.
<img width="1003" alt="Screen Shot 2022-02-12 at 2 41 05 PM" src="https://user-images.githubusercontent.com/49642360/153731113-22bd16a0-b291-4f94-a736-5c1715f856d4.png">




