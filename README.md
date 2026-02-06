# Currency Converter Web Application

A responsive and lightweight Currency Converter built using **HTML, CSS, and JavaScript**, integrating a real-time exchange rate API.
This project demonstrates practical implementation of API consumption, asynchronous JavaScript, DOM manipulation, and structured frontend architecture.


# Overview

This web application allows users to:

* Select a base currency
* Select a target currency
* Enter an amount
* Retrieve real-time exchange rates
* View the converted value instantly

Country flags dynamically update based on selected currencies, improving usability and visual clarity.

# Features

* Real-time currency conversion
* Dynamic dropdown population from currency list
* Country flag integration
* Input validation for invalid or empty values
* Asynchronous data fetching using `async/await`
* Clean and responsive user interface
* Error handling for API failures


# Technology Stack

* HTML5
* CSS3
* JavaScript (ES6+)
* Fetch API
* Exchange Rate API (CORS-enabled endpoint)
* FlagsAPI for country flag rendering


# API Integration

The application uses a public exchange rate endpoint:
https://open.er-api.com/v6/latest/{BASE_CURRENCY}

# Project Structure

Currency-Converter/
│
├── API.html        # Main HTML structure
├── style.css         # Styling and layout
├── Api1.js         # Core application logic
├── country.js          # Currency-to-country mapping object
└── README.md
```


1. On page load, dropdown menus are dynamically populated using a predefined currency list.
2. When a currency selection changes, the corresponding country flag updates.
3. On clicking the convert button:

   * Default form submission is prevented.
   * The application fetches exchange rate data based on the selected base currency.
   * The selected target currency rate is extracted.
   * The final converted amount is calculated and displayed dynamically.


During development, key challenges addressed included:

* CORS policy restrictions from certain APIs
* Handling invalid API keys
* Managing different API response structures
* Debugging asynchronous fetch failures

These were resolved by selecting a CORS-enabled endpoint and implementing structured error checks.

Shivam Kumar Shukla
B.Tech in Artificial Intelligence
