# BUSINESS CASE

The Ice cream company requires a solution where the customer can order ice cream (minimum 1 scoop) and an unlimited number of scoops in a dynamic manner. Customers should also be able to select the toppings, sprinkles and whether they would like to include a Waffer. The solution should also allow to automatically calculate the total price.

<u> Reports </u>

Ice selling history grouped by day.

<u> Dashboard </u>

- Ice cream selling history grouped by days.
- Top 5 flavours sold.

<u> Custom Homepage </u>

When users log onto Salesforce on their homepage the data from the reports should be displayed on the homepage with visual charts. It should also allow users to show recent records.

<hr>

# MY SOLUTION

## Step 1 - DETERMINE OBJECT USAGE

The solution was developed on the dev org instance [https://eu40.lightning.force.com/] (https://eu40.lightning.force.com/)

The first step during the process would be to ask yourself which standard objects can be used that would fulfill the requirements so this is what i came up with:

### CONTACTS

This will be used to register new and existing customers that want to order.

### OPPORTUNITIES

This will be used to register the sales of ice cream products.

### PRODUCTS

Goes without saying this would be required to register each ice cream flavour and toppings.

### PRICE BOOKS

We will be using only 1 price book as this Business Model only tragets individual customers, here we will be adding price per unit for ice cream and toppings.

## Step 2 - DEFINING THE AVAILABLE PRODUCTS

we search for Products object

[App Launcher](https://github.com/salv236/Salesforce-projects-and-challenges.git/images/app-launcher.png)



