# Retrieving data with Axios and Fetch

This project demonstrates how to use `axios` and `fetch` to retrieve data from an API and populate a dropdown menu with cat breeds. 
It also includes functionality to display more information about the selected breed in a carousel.

## Getting Started

### Prerequisites

- Node.js and npm installed
  
The API key for The Cat API is included in the project to facilitate its use. 

### Installation

1. Clone the repository:
    ```bash
    git clone <https://github.com/SilvinaFigueroa/api-with-axios/>
    cd <api-with-axios>
    ```

2. Install dependencies:
    ```bash
    npm install
    ```

### Usage

1. Start your local server:
    ```bash
    npm start
    ```

2. Open your browser and navigate to `http://localhost:1234` (or the port specified in your configuration).

## Project Structure

- `index.js`: Main JavaScript file that contains the functionality for fetching data and handling user interactions.
- `Carousel.js`: Module for handling carousel functionality.
- `index.html`: Main HTML file for the project.
- `styles.css`: CSS file for styling the project.

## Functionality

### Initial Load

The `initialLoad` function retrieves a list of cat breeds from The Cat API using `fetch` and `axios` and populates a dropdown menu with these breeds. 
You can uncomment the Axios section to use Axios or uncomment the Fetch section to try the implementation with Fetch. Both were included to showcase the differences.

```javascript
// -------API call with Fetch
// const result = await fetch(API_URL, {
//     headers: {
//         'x-api-key': API_KEY
//     },
// })
// let breeds = await result.json()

// -------API call with Axios
const result = await axios.get(API_URL)
let breeds = result.data
```


## Acknowledgments
[The Cat API](https://thecatapi.com/)

