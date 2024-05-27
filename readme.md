# Delivery Fee Calculator

This Python application calculates delivery fees using an HTTP API. It serves as a backend for handling delivery fee calculations depends on the cart value, the number of items in the cart, the time of the order, and the delivery distance.The project is uploaded as a zip drive on Google Drive for easy access and distribution.



## Table of Contents

- Features
- Google Drive Link
- Technologies Used
- Installation
- Usage
- API Documentation
- Dependencies
- License

## Features

- Calculate delivery fees based on parameters such as on the cart value, the number of items in the cart, the time of the order, and the delivery distance.

- Provide an HTTP API for easy integration into other systems.
## Google Drive Link

The project files, including the source code and documentation, can be found on Google Drive. [Link to Google Drive](https://drive.google.com/file/d/1Cy2VLLjJGslRp5Y7dcysaQ-bDfnxM-NU/view?usp=sharing).The folder contains the following files.

1.Delivery_fee_Calculator.py :This python file contain the methods for calculating delivery fee based on cart value,no.of items,distance and rush time (The rules followed as given in the preassignment task)

2.app.py:It is part of simple Flask application and serves as the main script to run the application.

3.__pycache__ :It is special directory in Python that is used to store compiled bytecode files (.pyc) generated by the Python interpreter

4.readme.md:


## Technologies Used

- **Programming Language:** Python 3.10.11
- **Web Framework:** Flask 3.0.1
## API Testing with Postman
To test the Delivery Fee Calculator API, you can use Postman. Follow these steps:

1. **Download and Install Postman:**
   If you don't have Postman installed, [download it here](https://www.postman.com/downloads/).

## Installation

1. Download and unzip the folder woltfinal.

## Usage

1. Start the application:

    ```bash
    python app.py
    ```

2. The application will now be running at `http://localhost:5000`.

## API Documentation

- Endpoint: `/Delivery`
- Method: `POST`
- Request body:

    ```json
    {"cart_value": 790, "delivery_distance": 2235, "number_of_items": 4, "time": "2024-01-15T13:00:00Z"}
    ```
   Description about values in the JSON request

    cart_value(Integer):Value of the shopping cart in cents.

    delivery_distance(Integer):The distance between the store and customer’s location in meters.

    number_of_items(Integer):The number of items in the customer's shopping cart.

    time(String):Order time in UTC in ISO format.
- Response:

    ```json
    {"delivery_fee": 710}
    ```
     delivery_fee(Integer):Calculated delivery fee in cents.

## Dependencies

- Flask 3.0.1
- Python 3.10.11
- pytz library #to work with time zones
## License

This project is licensed under the MIT License.