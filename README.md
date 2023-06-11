# EXP 06 - CREATE A SQL PROGRAM USING SET OPERATION
[ UNION , UNION ALL ,INTERSECT , EXCEPT ]

## AIM:

To create a sql program using set operation 

## ALGORITHM:

1) Create tables A and B with attributes ID and name
2) Insert values into the tables
3) Display the tables
4) Perform set operations
5) Union - Combines the distinct rows from both tables A and B
6) Union All - Combines all rows from both tables A and B, including duplicates
7) Intersect - Retrieves the common rows between tables A and B
8) Except - Retrieves the rows from table A that are not present in table B

## PROGRAM:
```
java
CREATE TABLE A (
    ID INT,
    name VARCHAR(50)
);

CREATE TABLE B (
    ID INT,
    name VARCHAR(50)
);
INSERT INTO A (ID, name) VALUES (1, 'John');
INSERT INTO A (ID, name) VALUES (2, 'Jane');
INSERT INTO A (ID, name) VALUES (3, 'Alice');

INSERT INTO B (ID, name) VALUES (2, 'Jane');
INSERT INTO B (ID, name) VALUES (3, 'Alice');
INSERT INTO B (ID, name) VALUES (4, 'Mike');
SELECT * FROM A;
SELECT * FROM B;
SELECT * FROM A
UNION
SELECT * FROM B;
SELECT * FROM A
UNION ALL
SELECT * FROM B;
SELECT * FROM A
INTERSECT
SELECT * FROM B;
SELECT * FROM A
EXCEPT
SELECT * FROM B;
```
## OUTPUT:

### TABLE A:

<img width="401" alt="image" src="https://github.com/Monisha-11/EXP-06---SET-OPERATION/assets/93427240/7163bcab-ce1b-463d-a87f-24fb279cd300">

### TABLE B:

<img width="396" alt="image" src="https://github.com/Monisha-11/EXP-06---SET-OPERATION/assets/93427240/1e264a41-8af7-448d-b6c3-4068dbc8fcc6">

### UNION 

<img width="410" alt="image" src="https://github.com/Monisha-11/EXP-06---SET-OPERATION/assets/93427240/fc0ce7a9-8186-4d2a-ba88-f10d823e85c6">

### UNION ALL:

<img width="413" alt="image" src="https://github.com/Monisha-11/EXP-06---SET-OPERATION/assets/93427240/731937b5-dbe7-4fd6-ac47-7931150213c3">

### INTERSECT:

<img width="389" alt="image" src="https://github.com/Monisha-11/EXP-06---SET-OPERATION/assets/93427240/961a19cf-b7a8-49d1-a9e3-dd898fd43d0e">

### EXCEPT

<img width="390" alt="image" src="https://github.com/Monisha-11/EXP-06---SET-OPERATION/assets/93427240/8861ae93-b662-436c-bfec-338751e597a2">

## RESULT:

Thus we have successfully obtained the required result using the above-given code.
