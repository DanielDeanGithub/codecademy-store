#### Objective provided by Codecademy

### FRONT-END DEVELOPMENT

# Codecademy Store

In this project, you’ll build a program that mimics Codecademy’s own online store! The application should display products from the Codecademy store and allow the user to add them to their cart. In the cart, the user can adjust the quantity of each item and the running total will be displayed at the bottom. Lastly, the user can choose the currency for the entire application.

![shopping-cart-demo](https://github.com/user-attachments/assets/31137365-6fbb-4331-9b13-3b969443450e)

This application has three slices of state:

  - `inventory`: An array of objects representing the items that are available to purchase.
  - `cart`: An object that maps the name of each item added to the cart to an object with the price and desired quantity for that item.
  - `currencyFilter`: A string that represents the currency used to calculate the prices displayed to the user: `'USD'`, `'CAD'` or `'EUR'`.

An example of this application’s state might look like this:

```js
state = {
  inventory: [
    { name: 'Hat', img: 'img/hat.png', price: 15.99 },
    { name: 'T-Shirt', img: 'img/t-shirt.png', price: 18.99 },
    { name: 'Hoodie', img: 'img/hoodie.png', price: 49.99 },
  ],
  cart: {
    'Hat': { price: 15.99, quantity: 0 },
    'T-Shirt': { price: 15.99, quantity: 2 },
    'Hoodie': { price: 18.99, quantity: 1 },
  },
  currencyFilter: 'CAD'
}
```


As you will see, the file structure has been organized using the recommended feature-based pattern and most of the inventory and currency features have been built for you. It will be up to you to:

  - complete the cart’s action creators and reducer logic
  - create the `store` using `createStore()` and `combineReducers()`
  - pass the `store` resources to presentational components via the top-level `<App />` component
  - render the `<Cart />` component using the current state data
  - dispatch actions to the `store`

Let’s get started!

If you get stuck during this project or would like to see an experienced developer work through it, click **“Get Unstuck”** to **see a project walkthrough video***.

>_Note: the output terminal below the coding area is there to display syntax errors and can be used when debugging your code. Feel free to minimize it when not in use._

Code review available when you’re done
