🌐 SimpleStorage DApp

A minimal decentralized application (DApp) built using Solidity, Ethers.js, and MetaMask.
Users can connect their wallet, store a value on the blockchain, and retrieve it — all through a sleek frontend interface.

Features

Connect MetaMask wallet

Store a number on the blockchain

Fetch the stored number anytime

Smart contract deployed on a test network

Fast, simple, beginner-friendly Web3 setup

📂 Project Structure
/SimpleStorage-DApp
│── index.html        # Frontend UI + Ethers.js logic
│── README.md         # Documentation
└── contract.sol      # Optional: Your Solidity smart contract

Smart Contract (Solidity)
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.0;

contract SimpleStorage {
    uint256 value;

    function set(uint256 _value) public {
        value = _value;
    }

    function get() public view returns (uint256) {
        return value;
    }
}


This contract lets you set and get a single number on the blockchain.

Technologies Used

Solidity — smart contract language

Remix IDE — deployed the contract

MetaMask — wallet for signing transactions

Ethers.js (v6) — interact with blockchain

HTML/CSS/JS — clean and simple frontend

How It Works

User opens the webpage

Clicks Connect Wallet

MetaMask opens → user approves connection

Enter a value → hit Set Value

Transaction is sent & confirmed on-chain

Hit Get Value → reads stored value

🔧 Configuration
1️⃣ Replace Contract Address

Inside index.html:

const contractAddress = "YOUR_DEPLOYED_CONTRACT_ADDRESS";

2️⃣ Add Your ABI

Paste the ABI from Remix:

const abi = [ ... ];

▶️ Run the DApp

You don’t need servers or anything fancy.

Just open the index.html file in your browser:

Right click → Open with → Chrome


Make sure:

MetaMask is installed

MetaMask is on the same network you deployed to (Sepolia / your testnet)

Screenshots

Add screenshots for extra ✨professional vibes✨:

Connect Wallet screen

Set Value

Get Value

MetaMask transaction popup

Contributing

Feel free to fork this project, improve it, or turn it into something wild — like adding events, mapping, or even NFTs 👀

Author

Built by Nandhana 
A curious learner stepping into the Web3 world.
