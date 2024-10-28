# API Genie

Welcome to **API Genie**!

A magical space for all API tests. 
This is your friendly genie for swift API testing.

This repository provides a flexible testing framework for API endpoints using Jest and Axios. With just a single JavaScript file, developers can easily set up their own API tests, ensuring reliability and efficiency in their development process.

## Features

- **Single Test File**: Contains all necessary testing logic without modification.
- **Easy Integration**: Use Axios for API requests and Jest for running the tests.
- **Customizable Configuration**: A sample `testConfig.js` is created for your reference. Modify the `testConfig.js` file to suit your specific testing needs. 

## Getting Started

To get started with API Genie, follow these steps:

### Prerequisites

Make sure you have [Node.js](https://nodejs.org/) installed on your machine.

### Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/yourusername/API-Genie.git
   cd API-Genie

2. **Install Dependencies**:
   ```bash
   npm install axios jest --save-dev
3. **Configure Your Tests**:
   
   Open the testConfig.js file and modify the settings according to your API requirements, including endpoints, methods, payloads, and expected responses.

### Running tests
Run the server.js before you run the following command. You can use:
```bash
node server.js
```
Once you’ve set up the testConfig.js file, you can run your tests using Jest:
```bash
npx jest test.spec.js
```
### File Structure
- test.spec.js: The main test file where the API tests are defined (unchanged).
- testConfig.js: Configuration file to customize your API testing.

### Example Configuration
Here’s a sample snippet of what your testConfig.js might look like:

```JavaScript
const indexTestConfig = require('path-to-your-controllerIndex');

const testConfig={
    testIndex: true
}
const testCases = [];
if (testConfig.testIndex) testCases.push(indexTestConfig);

module.exports={testConfig, testCases};
```
### Contributing

If you'd like to contribute to API Genie, please fork the repository and submit a pull request with your enhancements or bug fixes.

Happy Testing! 🚀
