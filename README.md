# blockchainForHealthcare20221001

1. Prepare Github Desktop app
2. Try to clone this repo into your github folder
3. Before starting the project, turn on Ganache and make sure your ehr project is running
4. Turn on IPFS Desktop app. If haven't install, the app can be download via https://docs.ipfs.tech/install/ipfs-desktop/
5. Open your favorite browser, and make sure MetaMask extension is logged in.
6. Open cmd from this repo/Blockchain For Healthcare 20221001 folder, then type the cmd "yarn start"

# Detailed Version of FYP Setup Guide
Step 1. Link to the video for installation purposes:
https://www.youtube.com/playlist?list=PL54V-i7zW55d1VKxEkp9DCPt5k_zE6m3X

Step 2. After following the video:
PS: The approach that we use is IPFS LOCAL!!
(Refer to this forum for IPFS config due to doctor cannot be added)

https://github.com/shamil-t/ehr-blockchain/issues/15

Step 3. Remember to download IPFS Distrubution in your pc and follow this below:
1. Open your IPFS distribution
2. Go to settings (on your bottom left on your software)
3. Scroll all the way down to IPFS Config
4. Copy and Paste it to IPFS Config (Refer to code below)

PS: find for HTTPHeaders at the IPFS config which is supposed to be around your 3rd line
of code.

Code:

"Access-Control-Allow-Methods": [
"POST",
"GET"
],
"Access-Control-Allow-Origin": [
"*"
]


Step 4. How to start Healthcare Project

1. Turn on Docker Desktop (not needed)
2. Turn on Ganache 
3. Go to Command Prompt
4. type and enter cd C:\Users\User\Desktop\FYP\ehr-blockchain
5. type and enter yarn start
6. once compiled successfully go to localhost:4200
7. go to metamask and renew the private key using ganache
8. change 'ETH Admin' private key to the ganache first key
9. save the work and connect the account with with localhost:4200
(it wont work if you connect metamask with different tabs)
10. open another cmd and type truffle migrate to activate contracts migrations and roles
11. type truffle deploy
12. head back to localhost:4200 and click on admin
13. here is the dashboard of EHR Project
