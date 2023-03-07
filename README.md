# CoffeeMachine-OOP
MenuItem Class
Attributes:
- name <br />
(str) The name of the drink. <br />
e.g. “latte” <br />

- cost <br />
(float) The price of the drink. <br />
e.g 1.5 <br />

- ingredients <br />
(dictionary) The ingredients and amounts required to make the drink. <br />
e.g. {“water”: 100, “coffee”: 16} <br />

Menu Class
Methods:
- get_items()<br />
Returns all the names of the available menu items as a concatenated string.<br />
e.g. “latte/espresso/cappuccino”<br />

- find_drink(order_name)<br />
Parameter order_name: (str) The name of the drinks order.<br />
Searches the menu for a particular drink by name. Returns a MenuItem object if it exists,
otherwise returns None.<br />

CoffeeMaker Class
Methods:
- report()<br />
Prints a report of all resources.<br />
e.g.<br />
Water: 300ml
Milk: 200ml
Coffee: 100g

- is_resource_sufficient(drink)<br />
Parameter drink: (MenuItem) The MenuItem object to make.<br />
Returns True when the drink order can be made, False if ingredients are insufficient.<br />
e.g.<br />
True

- make_coffee(order)<br />
Parameter order: (MenuItem) The MenuItem object to make.<br />
Deducts the required ingredients from the resources.<br />

MoneyMachine Class
Methods:
- report()<br />
Prints the current profit<br />
e.g.<br />
Money: $0

- make_payment(cost)<br />
Parameter cost: (float) The cost of the drink.<br />
Returns True when payment is accepted, or False if insufficient.<br />
e.g. False
