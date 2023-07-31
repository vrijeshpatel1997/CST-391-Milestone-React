# Design Report for Product Management App
# Vrijesh Patel
# CST 391
## Introduction
The Product Management App is a simple web application built using React for managing a list of products. The app allows users to view, add, edit, and delete products. It utilizes React Router for navigation and `react-bootstrap` for UI components. The app uses a local data file to store product information.

## Requirements
The design of the Product Management App was based on the following requirements:
1. Display a list of products with their Name, ID, and Price.
2. Allow users to add new products with a unique ID generated for each product.
3. Enable users to edit existing product details, including Name and Price.
4. Provide the ability to delete products from the list.

## Components
The app consists of four main components:
1. **Home Component**: Displays a table with the list of products fetched from the `Products` array. Provides buttons to edit or delete each product. Includes a "Create" button to navigate to the Add Component.
2. **Add Component**: Renders a form to capture user input for adding a new product. Validates the input fields (Name and Price) and adds the product to the `Products` array when the form is submitted.
3. **Edit Component**: Allows users to modify existing product details. Retrieves the initial values (Name and Price) of the selected product from `localStorage`. Updates the product information in the `Products` array when the form is submitted.
4. **Products Data File**: Contains an array of product objects, each with a unique `Id`, `Name`, and `Price`. Serves as a temporary data storage solution for the app.

## Data Management
Since this is a simple frontend application, the product data is stored in memory as an array within the `Products` data file. The `Products` array is modified directly within the Add and Edit components. However, in a real-world application, it's recommended to use a backend server or a database to store and manage product data securely.

## Navigation
React Router is used for handling navigation between different components. It provides seamless routing within the app and allows users to switch between the home page, create product page, and edit product page using client-side navigation.

## User Interface
The user interface is designed using `react-bootstrap`, a popular CSS framework. It ensures a responsive and visually appealing layout across different devices and screen sizes.


The Product Management App is a simple yet functional frontend application for managing product data. It demonstrates the usage of React, React Router, and `react-bootstrap` to build a responsive and interactive user interface. With further enhancements and backend integration, this app can be scaled for real-world product management scenarios.



Loom Video Link:

https://www.loom.com/share/88c55fed65e4455fada9d1e142b24fcf
