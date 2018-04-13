# IS623Project
Problem Description
The purpose of this project is to develop an interactive information system for a CD
warehouse. This system will enable the company to create an online ordering system
interface (between the company and its customers) for everyday transactions.
The database that we will create has two kinds of end-users: customers and company
employees. Customers have access to the company’s web site and should be able to open
accounts, do searches for the albums that they want to purchase, place orders, and check
the current status of their account balances. While searching for an album, customers may
know as little as the title of a hit song from the album to the name of the bassist of the group.
Therefore, customers should be able to make searches by using one of the following: group
name, album name, and song title. After finding the album that the customers want to buy,
they can put it in their shopping cart, and at the end of the session they can place an order.
At any time, the customers can check their order’s status and their account balance.
The company’s employees periodically check the database to identify the customers with
positive balance and send a bill. They are also interested to know about customers’
preferences. Then customers are informed about new releases according to their
preferences. When an order is received, an employee checks the availability of the albums.
If the albums are available, they are mailed to the customer right away, and the inventory
level is updated. Customers are informed about the shipment date, and their balance is
updated. If the albums are not available, the suppliers are contacted. The supplier with the
lowest cost and closest distance to the warehouse is chosen. At the beginning of each
month suppliers get a payment from the company. Products are shipped through UPS.
Database Design
We present the main entity types of this database. For each entity type, we provide some of
the corresponding attributes. Use this information in order to: (a) Build an Enhanced E-R
diagram; (b) Transform the Enhanced E-R diagram to a relational database. Identify the
primary key(s) and the foreign key(s) for each relation. Draw the relational integrality
constraints; (c) For each of the relations created, indicate its normal form. If the relation is
not in the 3NF, decompose it into 3NF relations.
1. Album: The main attributes are identification number, name, songs, members, release
date, warehouse location, quantity available, category, etc.
2. Customer: The main attributes are identification number, name, address, telephone
number, e-mail, credit card information, music preferences, password, balance, etc.
3. Order: The main attributes are identification number, order date, description, expected
delivery date, actual delivery date, payment type, payment amount, payment date, etc.
4. Supplier: The main attributes are identification number, name, address, telephone
number, current balance, etc.
Note the following: (a) Music preferences is a multi-valued attribute of the entity type
Customer; (b) Whenever an album is purchased from a supplier, the following is recorded:
purchase date, purchase price, quantity purchased. (c) When an album is ordered by a
customer, the price is recorded. The price of an album changes with time. (d) The attribute
Songs of the entity type Album is a multi-valued attribute. (e) Members is a multi-valued
attribute of the entity type Album.
Access Application Development
The following are some of the queries, forms, and reports one can create in order to
increase the functionality of the database:
Queries:
1. The following set of queries helps the management with cost analysis:
a. Create a query that calculates the average inventory level for each album. This
query should also present the average inventory holding cost.
b. Create a query that calculates the quantity purchased per month per album and
corresponding costs.
c. Create a query that calculates the total purchases made per month during the last
year.
d. Create a query that calculates the overall monthly expenses (inventory holding
costs and purchasing costs).
e. Create a query that calculates the revenues generated during the current month.
f. Create a query that calculates the revenues generated so far in the current year.
g. Create a query that prompts for the identification number of an album and returns
its sales during the current month.
h. Create a query that presents the current month’s profits.
2. The following queries help the managers with inventory management decisions:
a. Create a query that classifies the products into A, B, and C categories based on the
principles of ABC analysis (20% of the products in the inventory, category A
products, count for 80% of the value of the inventory).
b. Create a query that calculates for each album the Economic Order Quantity (EOQ).
c. Create a query that forecasts the next month’s sales based on information about
past months’ sales.
3. Create a query that prompts for the identification number of a product and returns the
current location of the product in the warehouse.
4. Create a query that identifies the top ten bestsellers of this CD warehouse.
5. Create a query that presents a list of albums released during the current month.
6. Create a query that prompts for the name of a song and returns the name and
identification number of the album that has the selected song.
7. Create a query that prompts for the name of a singer and returns the songs sung by the
selected singer and the name of the corresponding album.
8. Create a query that lists the names and addresses of all the customers who have a
positive balance.
9. Create a query that lists the names and addresses of all the customers who have made
late payments in the past10. Create a query that lists the names and addresses of the suppliers that have delayed
their shipment at least once.
Forms:
1. Create a user sign-in form together with a registration form for new users.
2. Create the following data entry forms that are used for database administrative
functions: albums, customers, orders, suppliers, etc. These forms allow the user to add,
update, and delete information about albums, customers, orders, suppliers, etc.
3. Create a form that allows the user to browse through the information about the albums.
The form presents the following: album identification number, title, release date,
category, vocalist, etc. Insert a subform that presents the names of the songs of the
selected album. Create another subform that presents the names of the members of the
group that composed the selected album.
4. Create a form that allows the user to search for a particular album based on the
following criteria: album name, name of the vocalist, name of a song, group name, etc.
Insert a command button that, when clicked-on, returns the top ten bestsellers. Insert a
command button that, when clicked-on, returns a list of the new releases.
5. Create a form that allows the user to browse through the information about the
customers of the warehouse. The form should present the following: identification
number, name, address, telephone number, current balance, etc. Insert a subform that
presents all the orders placed so far by the selected customer. The orders should be
sorted in a descending order of the delivery date. For each order, the subform should
present the following: order identification number, order date, description, expected
delivery date, actual delivery date, payment type, payment amount, and payment date.
6. Create a form that allows the user to browse through the information about the
suppliers. Use textboxes to present the following: supplier identification number, name,
address, telephone number, and current balance. Create a subform that presents a list
of the orders sent so far to the selected supplier. Sort the orders in a descending order
of the delivery date. For each order, present the following: order identification number,
order date, description, expected delivery date, actual delivery date, payment type,
payment amount, and payment date.
7. Create the following cost/revenue information form. One can use a tab control to
manage the information provided in this form. The information about the current month’s
costs can be grouped together; the information about the current month’s revenues can
also be grouped together; etc. Use the queries about cost/revenue analysis we
presented as a source of information needed to complete this form.
Design a logo for this database. Insert this logo in the forms created above. Pick a
background color for the forms and colors for the borders of the titles. Include the following
in the forms created: record navigation command buttons, record operations command
buttons, and form operations command buttons as needed.
Reports
1. Use the chart wizard to plot the following:
a. Total sales per month during the last twelve months.
b. Total revenues per month during the last twelve months.
c. Total earnings per month during the last twelve months
d. Total sales, total revenues, and total earnings per month per album category (e.g.,
rap music, classical music, etc.) during the last twelve months.
e. Annual earnings during the last ten years.
f. Average monthly inventory level during the last twelve months.
g. Inventory holding costs per month in the last twelve months.
h. Inventory holding costs per month per album in the last twelve months.
2. Report detailed information about the customer orders placed during the current month.
3. Report detailed information about the orders sent to suppliers during the current month.
4. Report detailed information about delayed orders.
5. Report detailed information about new album releases.
6. Report detailed information about the top ten bestsellers.
7. Use the label wizard to create labels containing the address of each customer and
supplier.
