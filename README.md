# Voxy's Login web page

  # Introduction

This project has as its main goal to test different scenarios on [Voxy’s platform](https://web-stage.voxy.com/v2/#/login/). Here, you will find:
- A Microsoft Excel file presenting a set of test cases for the web page;
- Automated tests using Cypress;

## First Steps

First and foremost, it is necessary to set the environment for running the automated tests. You must install the following technology:

#### Node.js:
You can download Node.js [here](https://nodejs.org/en/download/). Whatever it is your platform, you should choose the LTS version, which is more stable. 

## Installation

After this project is downloaded and the environment set, you must unzip the project folder.
Open Terminal at the workplace folder, and run: 
```bash
npm install
```

## Extensions 
Here it is a list of VS Code Extensions used for the development of this project:

- [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint). This extension statically analyzes your code to quickly find problems.
##### How to run ESLint:
Open Terminal at the workplace folder. Then, run the following commands:
```bash
npm install eslint
```
```bash
eslint --init
```
ESLint will ask some questions to find the better setup for the project. Here it is the answers you should choose for this project:
```bash
How would you like to use ESLint? · style
√ What type of modules does your project use? · esm
√ Which framework does your project use? · none
√ Does your project use TypeScript? ·Yes
√ Where does your code run? · browser
√ How would you like to define a style for your project? · guide
√ Which style guide do you want to follow? · standard
√ What format do you want your config file to be in? · JSON

If the terminal warns you to install some dependencies, the following message will be displayed:
√ Would you like to install them now with npm? · Yes
```


- [ES6 Mocha Snippets](https://marketplace.visualstudio.com/items?itemName=spoonscen.es6-mocha-snippets).



## Usage

The project has an Excel file with 6 test cases. Aimed to a higher quality of the login flow, these are the test cases:
1- Login with unsigned e-mail.
2- Login with unsigned mobile number.
3- Changing the page to French
4- Enter any e-mail address (ex: anaclara.oscar@gmail.com).
5- Verify that when filling the e-mail field with a mobile phone, the field considers it to be invalid.
6- Sending a message to Support

Since the main login flow cannot be reproduced, the scenarios were chosen by observing its level of importance.

### Running the automated tests

For the automated tests, you must run at the workplace folder:

```bash
npx cypress run
```
A Cypress window will start running. There you can select the preferred browser and tests you'd like to see the outcome.

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
