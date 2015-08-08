Barista-matic programming assignment

The application works as follows:

The Barista-matic machine has an inventory and a menu.

The menu has the default recipes of drinks given in the assignment. Every recipe has a reference to the inventory, this way it is able to check the drinks that can be made. Every time it gets ingredients to prepare a new drink from the inventory the amount decreases.

The inventory has an instance of every available ingredient, and it uses a prototype pattern, every time we request for an ingredient, if it is available, returns a new copy of it.

These ingredients are a subclass of the Drink class, the class we use to build drinks around. Every time we add an ingredient to a drink we wrap the drink with the new ingredient, decorating the drink. It uses the decorator pattern for this goal.