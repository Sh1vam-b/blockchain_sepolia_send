Sepolia ERC-20 Token Transfer
A minimal web dApp that sends ERC-20 tokens from the connected MetaMask account to a recipient on the Ethereum Sepolia testnet and waits for the transaction to be confirmed.

Built for the course Aktuelle Themen der Informatik (Blockchain track) at FH Technikum Wien.

Features
Connects to MetaMask and gets a signer for the selected account
Checks that the wallet is on Sepolia (chain ID 11155111)
Calls the token contract's transfer(to, amount) via a minimal ABI
Converts the amount with ethers.parseUnits, shows the transaction hash and waits for confirmation with tx.wait()
Clear status and error messages (missing MetaMask, wrong network, rejected transaction)
Tech stack
HTML / JavaScript (single file, no build step)
ethers.js v6 (BrowserProvider, Signer, Contract)
MetaMask
How to run
Install MetaMask, switch to the Sepolia test network and make sure the account holds some Sepolia ETH (for gas) and the token.
Adjust CONTRACT_ADDRESS, RECIPIENT_ADDRESS and AMOUNT_TO_SEND at the top of the script if needed.
Open index.html in your browser, click the button and confirm the transaction in MetaMask.
Testnet only – never use this with real funds.

Related projects
blockchain_sepolia_checker – current block height
blockchain_sepolia_balance – read an ERC-20 token balance
