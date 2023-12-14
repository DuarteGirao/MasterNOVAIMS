Final Deliverables: <br>
• A report that contains: <br>
1) cover page with the names of the team members;<br>
2) one-page description of the fictitious business process; <br>
3) a figure with the ERD. The names of the entities and its attributes must be visible in the ERD. <br>
• One single SQL script to recreate the database and the existing data on it.<br>
• One SQL script with the queries from literal F, including a comment about the efficiency of each query (interpretation of the query execution plan).<br>
<br>
<br>


Description <br>
A. Think about any commercial business process of a product or service that needs a relational database to work (e.g., online shops, booking systems, food delivery apps, restaurant management, etc). 
Describe it in 1 page.<br>
<br>
B. Design and create an ERD in MySQL workbench. Do not forget to consider the three normal forms 
when you design your database model. The names of the entities and its attributes must be visible 
in the ERD. Your ERD should not have less than 8 tables.<br>
<br>
C. Create two triggers: (1) one for updates (you can choose any updating process, for example, if a product is sold, the trigger may update the available stock of products). 
And (2) a trigger that inserts a row in a “log” table (your ERD should include a log table). For defence, you should have ready the scripts to demonstrate that the trigger works.<br>
<br>
D. Create a physical relational database based on your ERD.<br>
<br>
E. Insert some data into you newly created database (20 or 30 rows of transactions would be enough). 
Make sure that you have transactions that involve at least 2 consecutive years. If you want to add more than just a few rows, feel free to look for openly available dataset and/or generate random data.<br>
<br>
F. Using MySQL, write the queries to retrieve the following information:<br>
1. List all the customer’s names, dates, and products or services used/booked/rented/bought by these customers in a range of two dates.<br>
2. List the best three customers/products/services/places (you are free to define the criteria for what means “best”)
3. Get the average amount of sales/bookings/rents/deliveries for a period that involves 2 or more years, as in the following example. 
4. Get the total sales/bookings/rents/deliveries by geographical location (city/country).<br>
5. List all the locations where products/services were sold, and the product has customer’s ratings
(Yes, your ERD must consider that customers can give ratings).<br>
<br>
G. Your business process includes the generation of an INVOICE (the invoice in next page is just an example).
Create two views to recreate the information on the INVOICE, one view for the head and totals, one view for the details.
