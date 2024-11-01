## Overview
The **Meets More Integration** project is a Playwright repository designed to test the frontend of the Meets More application. This repository includes configurations for consistent coding styles and formatting across different environments.

## Getting Started
These instructions will help you set up the project locally for development and testing purposes.

## Prerequisites
Make sure you have the following installed:
- [Node.js](https://nodejs.org/) (version X.X.X)
- [npm](https://www.npmjs.com/) (comes with Node.js)
- [VS Code](https://code.visualstudio.com/) (recommended)

## Installation
1. Clone the repository:
```bash
git clone https://github.com/AlbrightQA/meets-more-integration.git
cd meets-more-integration
```

2. Install dependencies:
```bash
npm install
```

3. (Optional) Install recommended VS Code extensions:
   - Open the project in VS Code.
   - You will be prompted to install recommended extensions. Accept the prompt.

## Configuration
To set up the necessary storage state files for the project, you can create the following files in the `integration/storageState` directory:

1. **BusinessAccessToken.json**
2. **BusinessLoginState.json**

You can create these files using the following commands:

```bash
cd integration/storageState
New-Item -Name BusinessAccessToken.json -ItemType File
New-Item -Name BusinessLoginState.json -ItemType File
```

After creating these files, global.setup will be able to store the necessary information.

### Running Tests
To run the tests, navigate to the `integration` directory and use the following command:
```bash
cd integration
npx playwright test /tests
```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeature`).
3. Make your changes and commit them (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeature`).
5. Open a pull request.