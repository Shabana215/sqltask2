# sqltask2
### Expense Tracker
Create a table in MySQL
- Database
- Create TAble
  1. expense_id
  1. category
  1. date
  1. amount
  1. description
  1. payment_mode

| expense_id | category   | date     | amount | description         | payment_mode |
| ---| ---| --- | ---| --- | --- | 
|   190    | Food      |1-02-2003|6000   |Vegetables,milk     | Cash        |
|   191    | Newspapers|5-02-2003|1000   | Etimes newspaper    | Online      |
| 192 | Entertainment | 7-02-2003 | 1000 | Cable or net | Online|
| 193 | Traveling | 8-02-2003 | 3000 | Vacation | Online |
| 194 | School Fees | 15-02-2003 | 5000 | UKG | Cash |
| 195 | House Rent | 12-02-2003 |10000 | Housing allowances | Cash |
|196 | Groceries | 15-02-2003 | 7000 | Relliance | Online |
|197 | Clothing | 13-02-2003 | 6000 | Pantaloons shopping mall | Online |
|198 | Refreshments | 10-02-2003 | 2000 | Biscutes, chocolates etc., | Online |
| 199 | Miscellenious | 16-02-2003 | 8000 | Other Expenses | Cash |

## Create expense_tracker table
 ```sql
 create table expense_tracker(expense_id int, category varchar(20), date date , amount float, description varchar(20), payment_mode varchar(10));
 ```

## Insert rows in expense_tracker
```sql
insert into expense_tracker values((190, 'Food' , 1-02-2003, 6000 , "Vegetables,milk" , 'Cash' )
(191, 'Newspapers', 5-02-2003, 1000, 'Etimes newspaper',  'Online'  ),
(192, 'Entertainment', 7-02-2003, 1000, "Cable or net", 'Online'),
(193, 'Traveling', 8-02-2003, 3000, 'Vacation', 'Online'),
(194, 'School Fees',  15-02-2003, 5000, 'UKG', 'Cash'),
(195, 'House Rent', 12-02-2003, 10000, 'Housing allowances', 'Cash' ),
(196, 'Groceries',15-02-2003, 7000, 'Relliance','Online'),
(197, 'Clothing', 13-02-2003, 6000, "Pantaloons shopping mall", 'Online'),
(198, 'Refreshments', 10-02-2003, 2000, "Biscutes, chocolates etc", 'Online'),
(199, 'Miscellenious', 16-02-2003, 8000, 'Other Expenses','Cash'));
```
## To select all rows from expense_tracker
```sql
select * from expense_tracker;
```

## JSON
```json
{
"expense_id": 200, 
"category" : "Health checkup",
"date" : "11-02-2003",
"amount" : 4200,
"description" : "Doctor appointment and drugs",
"payment_mode": "online and cash"
}