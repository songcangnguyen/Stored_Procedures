# stored_procedures in Snowflake
## 1.Design data model: Star Schema 
    a. 1 fact table: product order transaction 
    b. 2 dim tables 
## 2. Create dimension tables (dim tables) 
    a. dimdate: contains date info 
    b. dim_product: contains product infor (created it from loading product_info.txt) 

## 3. Fact process steps 
    a. Load source file into Snowflake database without any transformation > prestg_product...
    b. Link dimtable info to process foreign keys in fact table 
