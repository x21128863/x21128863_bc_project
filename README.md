
# x21128863_bc_project
The process of execution is taken in the following two steps: using source code located at:
 https://github.com/x21128863/x21128863_bc_project.git
A. Setting up the environment
    1. The '.env' file is the environment variable file to set up the contract details, 
        a. INFURA_TOKEN: this is the token associated with the Infura endpoint
        b. CONTRACT_ADDRESS : this is the address of deployed contract using remix.
        c. OWNER_ADDRESS: the metamask account address for the Ropstein test network.
        d. SUPER_SECRET_PRIVATE_KEY : this is the metamask account private key, to authorize the program to run the transactions.
    2. The ABI, of the deployed contract, needs to be copied to the 'const abi' variable in contract.js (this will be the same as already in code for the same standard contract) 
    3. update the accounts.txt file with the addresses where these token needs to be distributed.
B. Running the code for token distribution
    1. Navigate to the folder inside the current folder X21128863_ProjectCode

        > cd .\X21128863_ProjectCode

    2. The code is packaged as a Node package, just 'npm install' in the project folder will download all the following dependencies,as registered in package.json.
        a. "big-number": "^2.0.0",
        b. "dotenv": "^16.0.0",
        c. "ethereumjs-tx": "^2.1.2",
        d. "web3": "^1.7.1"'

        > npm install

    3. once all dependencies are downloaded, run 'npm start' The npm start command in term runs the invoking file 'distribute.js' using 'node distribute.js' as registered in package.json.
            
        >npm start
