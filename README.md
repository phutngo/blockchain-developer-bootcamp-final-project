# Final Project - NFT Collection Generator (NCG)

## Overview

There is a high demand from artists to share their creativity by producing large collections of semi-generative art that combines layers of images into many different holistic images. These artists have the skills to create the individual layers of images, but they lack the skills and tools to turn these individual images into a large collection of holistic images. For example given 10 layers of images and 10 variations per layer, the artists want to create 10000 NFT's.

This project is to create a lean pipeline that turns these layers of images into a large collection of NFTs (e.g. 10000 NFTs) that are browsable and buyable through a website.

## Features

### Module 1 - Image Processing/Generating
1. Given _n_ layers with each layer having _m_ variations, merge all the layers into random images which is a subset of _n^m_ images.
2. Produce metadata for these images that fit [Opensea Metadata Standards](https://docs.opensea.io/docs/metadata-standards).
3. Allow config that a specific variation only shows up if another variation shows up.
4. Allow config that a subset of the n layers must be unique. Example, you want your images to be unique without counting the background. Without the config if we do a naive way there would be images that are identical but with different backgrounds.
5. Provide summary statistics such as rarity of each variation.
6. Fast enough to produce 10000 images that are of decent resolution such as 1200x1200px.

#### Techstack
Node.js

### Module 2 - Smart Contract / Backend
1. Programatically upload the images to IPFS
2. Deploy the images collection as NFTs on the Ethereum Blockchain using OpenZeppelin smart contract templates for [ERC 721](https://docs.openzeppelin.com/contracts/4.x/api/token/erc721)
3. Optional/Bonus - Programatically post images for sale on opensea/rarible
4. Optioanl/Bonus - Lazy minting

#### Techstack
Node.js
Solidity
Truffle React Box?
Scaffold Eth?
Web3js or ethersjs?
hardhat or truffle?


### Module 3 - Frontend
1. A React frontend where users can see the images collection
2. Users can filter based on the layers and each variations
4. User can click "buy button" on the NFT and metamask opens. We load the appropriate transaction data and our smart contract address into Metamask for user to submit the transaction.
5. The NFT is then assigned/transferred to user's eth account.
6. Our website updates - by putting a SOLD sticker on the NFT's has been sold

#### Techstack
1. React
2. Material UI
3. Zustand (for state management)



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
