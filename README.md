# Get-User

This project is a web application developed using various technologies to create a user-friendly and interactive interface. It allows for adding and listing users with their information.

## Tech Stack

- HTML
- CSS
- JavaScript
- Bootstrap 5.3.0-alpha3
- Faker.js
- Superagent

## Features

### Add Users

The "Add Users" functionality allows you to generate random user data using the Faker.js library and add it to the server.

- Clicking the "Add Users" button triggers the `add()` function in the `script` tag.
- The `add()` function generates random user data using Faker.js, including name, email, username, password, phone, address, latitude, longitude, and date of birth.
- The generated user object is sent as a POST request to the server using Superagent.
- The server receives the user data and stores it in the database (LowDB).

### List All Users

The "List All Users" functionality retrieves the stored user data from the server and displays it in a formatted or raw format.

- Clicking the "List All Users (formatted)" or "List All Users (raw)" link in the navigation menu triggers the `data()` function in the `script` tag.
- The `data()` function sends a GET request to the server to fetch the user data.
- The server responds with the user data, which is then displayed on the webpage.

## Getting Started

1. Clone the project repository.
2. Install the dependencies by running `npm install`.
3. Start the server by running `node http_server.js`.
4. Open the web application in your browser.

## Project Structure

- `index.html`: The main HTML file that contains the structure and layout of the web application.
- `styles.css`: The CSS file that provides styles and design for the web application.
- `http_server.js`: The server-side JavaScript file that handles requests and stores user data using LowDB.
- `db.json`: The JSON file that serves as the database for storing user data.

## Dependencies

The project requires the following dependencies, which are automatically installed by running `npm install`:

- faker-js/faker: ^7.6.0
- body-parser: ^1.20.2
- express: ^4.18.2
- lowdb: ^1.0.0
- superagent: ^8.0.9

## Contributing

Contributions to the project are welcome. If you have any suggestions or improvements, feel free to submit a pull request.

## License

This project is licensed under the ISC License. You can find more details in the [LICENSE](LICENSE) file.

