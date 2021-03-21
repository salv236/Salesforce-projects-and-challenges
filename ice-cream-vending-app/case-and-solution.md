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

we search for Products object by going to the app launcher at the top left of the org

<img src="./images/app-launcher.png"/>

We then search for products

<img src="./images/search-for-products.png"/>

We should now see the products page clicking on the new button will allow us to start adding new products

<img src="./images/new.png"/>

We insert each product until all products have been added to the system. Adding new products by clicking **save & new** and clicking on **save** when we have decided its the last product.

product code naming convention starts with ice-001 where the last 3 digits increments +1

<img src="./images/ice-cream.png"/>

<img src="./images/all-ice-creams.png"/>

## Step 3 - INSERT THE PRODUCTS INTO THE PRICE BOOK

Within our applauncher we now search for price books

<img src="./images/search-for-price-books.png"/>

We are then taken to the main page of price books where we are shown the standard Price Book which is the default price book. We will not be required to insert additional price books as our base target is individual customers where we will have one dedicated fixed price.

<img src="./images/price-books-main-screen.png"/>
