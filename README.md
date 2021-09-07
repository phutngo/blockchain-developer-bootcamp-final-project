# Final Project - Generative NFT Collection

[Link To This Project Repo](https://github.com/phutngo/blockchain-developer-bootcamp-final-project)

[Final Project Ch1 Instructions](https://courses.consensys.net/courses/take/blockchain-developer-bootcamp-registration-2021/surveys/26729108-exercise-your-final-project-idea)

## Overview

Ultimately, I want to create a lean process to generate NFT collections.
This final project can be the proof of concept for this.

## Features

1. Images Generator - Given a set of attributes as image layers - merge the attributes together to generate the final art and corresponding metadata.
2. Host images - Bonus points if images are hosted on IPFS
3. Deploy the images collection as NFTs on the Ethereum Blockchain using openzeppelin smart contract templates for [ERC 721] (https://docs.openzeppelin.com/contracts/4.x/api/token/erc721)
4. Optionally post them for sale on opensea/rarible. 
5. Optionally lazy minting.
6. Front End - React - users can see the images collection.
   1. Users can filter based on attributes. 
   2. NFT's that are not available for purchase (because it's been sold) are dimmed.
   3. User can click "buy button" on the NFT and metamask opens. We load the appropriate data package and our smart contract address into metamask for user to submit the send transaction.
   4. The NFT is then assigned/transferred to user's eth account.


### Techstack
1. React
2. Material UI
3. Zustand for state management
4. NodeJS
5. Solidity
6. Web3js or ethersjs?
7. hardhat or truffle?


## Final Project Checklist

[Final Project Requirements](https://courses.consensys.net/courses/take/blockchain-developer-bootcamp-registration-2021/assignments/27500647-final-project-submission)

Please answer the following questions. Does your project:

1. [ ] Follow this naming format: https://github.com/YOUR_GITHUB_USERNAME_HERE/blockchain-developer-bootcamp-final-project? YES/NO

2. [ ] Contain a README.md file which describes the project, describes the directory structure, and where the frontend project can be accessed? YES/NO

3. [ ] Contain smart contract(s) which:
--Are commented to the specs described by NatSpec Solidity documentation
--Use at least two design patterns from the "Smart Contracts" section
--Protect against two attack vectors from the "Smart Contracts" section with its the SWC number
--Inherits from at least one library or interface
--Can be easily compiled, migrated and tested? YES/NO

4. [ ] Contain a Markdown file named design_pattern_decisions.md and avoiding_common_attacks.md? YES/NO

5. [ ] Have at least five smart contract unit tests that pass? YES/NO

6. [ ] Contain a `deployed_address.txt` file which contains the testnet address and network where your contract(s) have been deployed? YES/NO

7. [ ] Have a frontend interface built with a framework like React or HTML/CSS/JS that:
--Detects the presence of MetaMask
--Connects to the current account
--Displays information from your smart contract
--Allows a user to submit a transaction to update smart contract state
--Updates the frontend if the transaction is successful or not? YES/NO

8. [ ] Hosted on Heroku, Netlify, or some other free frontend service that gives users a public interface to your decentralized application? (That address should be in your README.md document) YES/NO

9. [ ] Have a folder named scripts which contains these scripts:
--`scripts/bootstrap` When run locally, it builds or checks for the dependencies of your project.
--`scripts/server` Spins up a local testnet and server to serve your decentralized application locally
--`scripts/tests` Used to run the test suite for your project? YES/NO

10. [ ] A screencast of you walking through your project? YES/NO