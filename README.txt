# Breelef.github.io

Brugere:
 
USERNAME: AdminUser PASSWORD: Password123!
USERNAME: WriteUser PASSWORD: Password123!
USERNAME: ReadUser PASSWORD: Password123!
 
(USING SQLCMD)
Open CMD using "kør som administrator"
choco install sqlcmd
 
add: "C:\Program Files\SqlCmd\" to the Path system enviromental environment
 
Open CMD og kør denne kommando med de forskellige brugere og se hvad de har tilladelse til
sqlcmd -S system-integration.database.windows.net -d granular_access -U USERNAME -P PASSWORD
 
SELECT QUERY
SELECT * FROM Items
 
INSERT QUERY
INSERT INTO Items (Name, Quantity) VALUES ('navn', 'antal');
 
GO SETUP:
Write "go" after every query
 
Database setup
 
Database:
granular_access
 
Table:
Items
 
Items:
data_id = PK/int
Name = varchar
Quantity = int
 
TASK:
5 items ialt som jeg gerne vil have navn og antal på i første omgang, og så skal der laves et nyt Item entry, med et givet navn og antal
