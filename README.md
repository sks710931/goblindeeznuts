
# Run the Frontend application

1. Clone this repository in your system
2. make sure you have nodeJs > 12.0 installed in your system, can check by running "node --version" in terminal
3. In terminal open the cloned folder 
4. run the command "npm install"
5. run the command "npm start" this will start the front end application, it uses the test version of the contract deployed at https://testnet.snowtrace.io/address/0x12fb4c3eB02BF18CE8641e0f66A98f653daf8759


# Deploying the Frontend Application and the contract
1. Copy the contract code from "src/contract/ERC721A.sol" file
2. open https://remix.ethereum.org
3. paste the complete contract code in one file and compile the code 
4. go to deploy contract menu, in the base uri constructor field provide the uri https://ipfs.io/ipfs/QmcCv6AthghDsxG2h7fAiTgDbvUucxRaCeNQFuCpumFZfH/ and hit deploy button.
5. copy the deployed contract address
6. go to the src/connectors/address.js file and replace the NFTContractAddress value with the address copied.
7. get the AVAX mainnet rpc url and in src/connectors/address.js update the rpc value with it
8. run npm start and make sure everything is running correctly
9. run command "npm build" to build the project
10. copy the contents of the /build folder and upload it to your web server
