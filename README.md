# User Guide for the Online Voting System using Blockchain

Welcome to the Online Voting System based on Ethereum blockchain technology. This guide will walk you through the steps to set up the development environment, register as a voter, and participate in the election. Please follow the instructions carefully.

## Setting up the Development Environment

Before you can start using the Online Voting System, you need to set up the development environment. Follow these steps:

### Requirements

- [Node.js](https://nodejs.org) installed on your computer.
- [Truffle](https://www.trufflesuite.com/truffle) framework installed globally using Node Package Manager (npm).
- [Ganache](https://github.com/trufflesuite/ganache-cli) (CLI) installed globally using npm.
- [Metamask](https://metamask.io/) browser extension installed.

#### Getting the Requirements

1. **Install Node.js:**
   Download and install Node.js from [here](https://nodejs.org/en/download/ "Go to official NodeJS download page.").

2. **Install Truffle and Ganache-cli:**
   Open your terminal (or command prompt) and run the following commands:

   ```shell
   npm install -g truffle
   npm install -g ganache-cli
   ```

3. **Install Metamask:**
   Download and install Metamask from [here](https://metamask.io/download "Go to official Metamask download page.") as a browser extension.

### Configuring the Project for Development

1. **Clone the Repository:**
   Open your terminal (or command prompt) and run the following command to clone the project repository:

   ```shell
   git clone https://github.com/akashroy1/VotingPlatform-BKT3001.git
   cd VotingPlatform-BKT3001
   ```

2. **Run Local Ethereum Blockchain (Ganache):**
   Start the local Ethereum blockchain using Ganache by running the following command:

   ```shell
   ganache-cli
   ```

   > Note: Keep the `ganache-cli` running as the blockchain network needs to be active all the time during development.

3. **Configure Metamask:**
   - Open your browser with Metamask installed.
   - Click on the Metamask extension icon.
   - Select "Import Account" and use the private keys from Ganache to import accounts into Metamask.

4. **Deploy Smart Contract:**
   In the terminal, navigate to the project root directory (`VotingPlatform-BKT3001`) and deploy the smart contract to the local blockchain network using Truffle:

   ```shell
   truffle migrate
   ```

   > Note: If you want to redeploy the contract, use `truffle migrate --reset`.

5. **Launch the Development Server (Frontend):**
   Now, navigate to the `client` directory and start the development server for the frontend:

   ```shell
   cd client
   npm install
   npm start
   ```

## User Registration and Voting

1. **Access the Online Voting System:**
   Open your web browser and navigate to the URL displayed when the frontend development server is running (`localhost:3000` by default).

2. **Register as a Voter:**
   - Connect your Metamask to the website.
   - Click on the "Register" button to register as a voter.
   - Fill in your details, including your blockchain account address, name, and phone number.
   - Click on "Register" to submit your details.

3. **Approval by Admin:**
   - The system admin will verify your registration details.
   - Once approved, you will be eligible to participate in the election.

4. **Cast Your Vote:**
   - Once the election starts, log in with your registered account.
   - Click on the "Vote" button to cast your vote for your preferred candidate.
   - Confirm the transaction in Metamask.

5. **Election Results:**
   - After the election ends, the admin will close the voting.
   - The results will be displayed on the website, and the winner will be announced.

Made with ❤️ by Akash, Samme, Jashwanth, Gourav.
