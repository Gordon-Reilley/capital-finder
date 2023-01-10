# Lab 16 - Serverless Functions

## Project Name - Capital Finder

### Author - Gordon P Reilley Jr

### Feature Tasks and Requirements:

- Create a serverless function following Vercel’s get-started directions that handles two kinds of queries:
  - The serverless function should handle a GET http request with a given country name that responds with a string with the form The capital of X is Y
  - E.g./capital-finder?country=Chile should generate an http response of The capital of Chile is Santiago.
  - The serverless function should handle a GET http request with a given capital that responds with a string with the form The capital of X is Y
    - E.g./capital-finder?capital=Santiago should generate an http response of Santiago is the capital of Chile.

### Example Urls

- `https://capital-finder-gordon-reilley.vercel.app/api/capital_finder?country=mexico`
  - Returns: The capital of Mexico is Mexico city.
- `https://capital-finder-gordon-reilley.vercel.app/api/capital_finder?capital=mexico%20city`
  - Returns: Mexico city is the capital of Mexico.
- If user enters something that isn't a country or capital
  - Returns: `Please enter a valid country or a capital.`