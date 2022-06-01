# Web App Security

## Many-to-many
#### Many-to-many relationships are the most commonly used table relationships. They provide crucial information, such as which customers your salespeople have contacted and which products are in customer orders. A many-to-many relationship exists when one or more items in one table can have a relationship to one or more items in another table. For example:

- Your Order table contains orders placed by multiple customers (who are listed in the Customers table), and a customer may place more than one order.

- Your Products table contains the individual products you sell, which are part of many orders in the Order table.

- One order may include one instance (or more than one instance) of a specific product and/or one instance (or more than one instance) of multiple products.

![Many-to-many](https://user-images.githubusercontent.com/97638932/161444337-4243fe88-4355-4d6f-8587-ecaed25c23de.png)


## Example 1: University Database
#### In this example, your task is to build a university database. You’ve just started, but you’re already stuck. You have to show the professors and the subjects they teach, but how will you do it?

#### Let me show you how to represent this relationship by first defining the entities. One should be the professor entity, and the other is subject. Let’s check if this could be a many-to-many relationship. One professor could teach one or many subjects, but one subject could also be taught by one or many professors. It seems it is an M:N relationship, so here’s how your logical model should look:
![Untitled](https://user-images.githubusercontent.com/97638932/161444818-f34c011d-a54f-42a7-99bc-3bc54acadadf.jpg)
