<!-- PROJECT LOGO -->
<br />
<p align="center">


  <h1 align="center">Budget Taker</h1>

  <p align="center">
    <a href="https://github.com/mygithub23/budget-tracker"><strong>Explore the docs »</strong></a>
    <br />
    <br />

  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary><h2 style="display: inline-block">Table of Contents</h2></summary>
  <ol>
    <li>
      <a href="#Screenshot">Screenshots</a>
      <ul>
        <li><a href="#Demo">Project Demo</a></li>
      </ul>
    </li>
    <li>
      <a href="#Short-Description">Project Objective</a>
      <ul>
        <li><a href="#Project-Description">Project Description</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#Technologies">Technologies</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#How-to-test">How to Test</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>

##Title

# Budget Taker

## Screenshots

 <p align="center">
    <a href="https://github.com/mygithub23/budget-tracker"><strong>Explore the project on Github »</strong></a>
  </p>
  <div>
    <img src="./assets/img/budget.gif">
  </div>
  <div>
    <img src="./assets/img/offline2.jpg">
</div>

### ✨Demo

Project Link: [https://fan1-budget-tracker.herokuapp.com/](Explor the project on Heroku)
<br>

<!-- ABOUT THE PROJECT -->

## Project Objective

Budget tracker application will help customers to keep track of their budget. This app allows users to add and substract transactions. The Budget app records each transaction and date and time of the transaction also it display all debit and credit ordered by date of the transaction. On the top of the app it displays the balance of user's account.

## Preject Description

The central feature that distinguishes the REST architectural style from other network-based styles is its emphasis on a uniform interface between components (Figure 5-6). By applying the software engineering principle of generality to the component interface, the overall system architecture is simplified and the visibility of interactions is improved. Implementations are decoupled from the services they provide, which encourages independent evolvability. The trade-off, though, is that a uniform interface degrades efficiency, since information is transferred in a standardized form rather than one which is specific to an application's needs. The REST interface is designed to be efficient for large-grain hypermedia data transfer, optimizing for the common case of the Web, but resulting in an interface that is not optimal for other forms of architectural interaction.

### Prerequisites

Need access to Internet to install all project dependencies.

## Technologies

Nodejs, Express, mongodb, Atlas and mongoose

## Database
create a collection on mongodb database

```
mongoose.connect(process.env.MONGODB_URL|| "mongodb://localhost:27017/budget", {
    useNewUrlParser: true,
    useFindAndModify: false,
    useCreateIndex: true,
    useUnifiedTopology: true
});


const mongoose = require("mongoose");

const Schema = mongoose.Schema;

const transactionSchema = new Schema(
  {
    name: {
      type: String,
      trim: true,
      required: "Enter a name for transaction"
    },
    value: {
      type: Number,
      required: "Enter an amount"
    },
    date: {
      type: Date,
      default: Date.now
    }
  }
);

const Transaction = mongoose.model("Transaction", transactionSchema);

module.exports = Transaction;

```

## Installation

on project root directory type 
```
$ npm install

$ npm start
```
## Usage

```
How to use the project - We can use Inquirer for this. The module includes a number of methods for various types of prompts, which are roughly analogous to HTML form controls. In order to collect the user’s GitHub username and password, we’re going to use the input and password types respectively.
```

## How to test

```
how to test the project - Require steps We can use Inquirer for this. The module includes a number of methods for various types of prompts, which are roughly analogous to HTML form controls. In order to collect the user’s GitHub username and password, we’re going to use the input and password types respectively.
```

<!-- LICENSE -->

## License

This project is [MIT](https://choosealicense.com/licenses/MIT/) licensed.<br />

Copyright © 2021 [Ali Alaoui}](https://github.com/mygithub23})

<!-- CONTACT -->

## Contact

Contact the author with any questions!<br>

- Twitter: [@myTwitterHandle](https://twitter.com/@myTwitterHandle)
- Github link: @[mygithub23](https://github.com/mygithub23)<br>
- Email: ali.alaoui@gmail.co
- heroku: https://notes-taker-manager.herokuapp.com/
- heroku git: https://git.heroku.com/notes-taker-manager.git
