# Bamazon

Bamazon is a backend application which utilizies MySQL and node.js to provide an online shopping and inventory management experience.  When running the bamazonCustomer.js file in node, the user is given the option to:
1.  Browse and Buy
2.  Manage Inventory

If the user selects the first option, he or she will see the output of items maintained in the MySQL database including the item number, the name of the product, and its price.  The user then types in the number corresponding to the unit he or she would like to buy, and enters the quantity.

If the quantity requested is greater than the inventory, a message appears informing the user that there is not enough inventory to satisfy the purchase, and another selection must be made.  If, however, the requested quantity is in stock, the user will be shown the total price of the item, and the requested quantity will be deducted from the number of items in stock.

If at the main menu, the user selects the option to "Manage Inventory," the user is presented with following options:
1.  View Products
2.  View Low Inventory
3.  Add to Inventory
4.  Add New Product

View Products: Just as in the in the Browse and Buy selection, if the user selects "View Products" he or she will be countenanced with an output generated by SQL query of the various products available, this time also including the amount in stock.

View Low Inventory: Selecting this command initiates a function which will return any item that has less than 300 units available.

Add to Inventory: As the name would suggest, this option allows the user to select which item needs to be re-stocked and by how many units, resulting in an UPDATE statement to increase the inventory of the unit in question by the quantity specified.

Add New Product: This selection will ask the user the name, department, price, and quantity of the item he or she would like to add to the product line.  On submit, an INSERT statement is run to add the new product to the products table.

Screen shots for the various features enabled through this application can be found here: https://docs.google.com/document/d/12hgU-5kdpCT24SD_3c6JdLat0X60tv6DXXQCXjlv0XA/edit?usp=sharing
