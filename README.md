# Ethereum's Solidity smart contract + Flask App

This repository hosts a blockchain-based voting application, leveraging Ethereum's Solidity smart contracts and a Flask web server. The project demonstrates a simple yet effective voting system where users can cast votes for predefined candidates and view results.

## Project Overview
### Smart Contract
Developed in Solidity, the Voting smart contract is the backbone of this application. It features functionalities such as adding candidates, casting votes, and preventing double voting.

The smart contract is deployed and tested on a local Ethereum blockchain using Ganache, ensuring a controlled and safe development environment.

### Flask Application
The Flask web server serves as the interface for user interaction with the smart contract.

It includes routes for displaying candidates, casting votes, and viewing election results, all by interacting with the Ethereum blockchain.

## Features

Simple and Intuitive UI: The Flask app provides a user-friendly interface for interacting with the voting system.

Secure Voting Mechanism: The smart contract ensures secure voting, with checks against double voting and validation of candidate IDs.

Local Blockchain Simulation: Utilizes Ganache for a simulated Ethereum blockchain environment, ideal for development and testing.

## Prerequisites

Flask: User Interface 

Node.js and npm: Required for managing blockchain development tools.

Ganache: A personal blockchain for Ethereum development.

Truffle Suite: For compiling, testing, and deploying the Solidity smart contract.

## Usage

- ganache-cli --port 7545
- replace private_keys in app.py with the ones generated by previous command
- truffle compile
- truffle migrate --reset
- replace contract_address in app.py with the one given by previous command ("2_deploy_contracts.js" contract number)

Casting Votes: Access the main page, choose a candidate and submit your vote.

Viewing Results: Navigate to the results endpoint to see the current vote tallies.

## Tests
The Solidity smart contract includes comprehensive tests covering various scenarios like voting validation and event emission.

Run tests with "truffle test" to ensure the integrity of the smart contract.
