# CASSANDRA COLUMN FAMILY DATABASE
RESTAURANT  FOOD ORDERING SYSTEM :

  Restaurant food ordering system is used to automate menu for ordering food in restaurants .
 In these modern days the number of restaurants are increasing. They also require very fast processing for serving food to the customers.
 With the increasing number of customers, it would require more man power, since the current situation has become hectic for the restaurants.
 Also changes in the hardcopy of the menu can’t happen . For these problem ,restaurant food ordering system was proposed.
         
CASSANDRA:

 Cassandra is a column-family database that stores data in rows with column families.
Cassandra provides tunable consistencythat allows to balance consistency and availability.

KEY VALUE TO COLUMN-FAMILY:

 To convert the REDIS KEY VALUE database into a CASSANDRA COLUMN FAMILY database,
    
            STEP-1:Create a keyspace in Cassandra to store the data.
            STEP-2:Create column families to store the data.
            STEP-3:Insert the data into the column families.
OPERATIONS:

-> Created a KEYSPACE called "hotel".

-> Cassandra CRUD operations stands for Create,Read,Update and Delete or Drop.

-> To create a table,the following syntax is used:
        
       CREATE TABLE <tablename> (attribute1 attributetype,attribute2 atrributetype,.......,atrributeN attributetype);
-> To read a table,the following yntax is used:
       
       SELECT * FROM <tablename>;
-> To update a data in a table,the following syntax is used:
       
       UPDATE <tablename> SET <attributename>=<'newvalue'> WHERE <condition>;
-> To delete a particular data in a table,the following syntax is used:
        
       DELETE FROM <tablename> WHERE <condition>;
-> "describe" command is used to provide the information about the connected Cassandra cluster and objects within the cluster.
        
       describe <tablename>;
ATTRIBUTES DETAILS :

       For Restaurant food ordering system,it contains six tables named,
       
             1.customer
             2.order 
             3.menu
             4.fooditem
             5.payment
             6.administrator     
             
     The "customer" table contains the information about the customers.
     The following are the attributes in the customer table:
     
              ->custid represents the customerid.
              ->custname represents the customername.
              ->email represents the customer emailid.
              
     The "order" table contains the information about customer order.
     The following are the attributes in the order table:
     
              ->orderid
              ->custid represents the customerid.
              ->quantity represents the quantity ordered by the customer.
              
     The "menu" table contains the information about food menu.
     The following are the attributes in the menu table:
     
              ->menuid
              ->foodid
              
     The "fooditem" table contains the details of the food in the restaurant.
     The following are the attributes in the fooditem table:
     
              ->foodid
              ->itemcategory represents varieties of food item categories.
              ->name represents food name.
              
    The "payment" table contains the details of payment processing.
    The following are the attributes in the payment table:
    
              ->custid represents customerid.
              ->orderid 
              ->paymenttype represents online payment including gpay,paytm and cash on delivery as cod.
              
    The"administrator"table contains informations about the persons who manages the ordering system of the restaurant.
    The following are the attributes in the administrator table:
    
              ->adminid represents administrator id.
              ->name represents administrator name.
              ->username
              ->password
              
CONCLUSION:

  Column-family databases are a powerful tool in the world of data management, 
  and their popularity is only expected to grow as organizations continue to generate and collect more and more data.
