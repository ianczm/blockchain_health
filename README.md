# blockchainForHealthcare20221001

# Prerequisite
1. Windows 10 machine or virtual machine
2. Git
3. Node.js
4. Already following the videos in this playlist, from part 1 to part 7

https://www.youtube.com/playlist?list=PL54V-i7zW55d1VKxEkp9DCPt5k_zE6m3X

After following the videos, your pc should already have:

i. Ganache

ii. Google Chrome with Metamask

5. IPFS Desktop
6. Github Desktop

# Installation
1. Change IPFS Settings

a. Open your IPFS distribution

b. Go to settings (on your bottom left on your software)

c. Copy and Paste the following code to HTTPHeaders in IPFS Config

"Access-Control-Allow-Methods": [
	"POST",
	"GET"
],
"Access-Control-Allow-Origin": [
	"*"
]

2. Use Github Desktop app to clone this repo into your github folder
3. Turn on Ganache and make sure your ehr project is running
4. Open your browser, and make sure MetaMask extension is logged in.
5. Open cmd from this 'repo/Blockchain For Healthcare 20221001' folder, then type the cmd "yarn start"
6. go to metamask and renew the private key using ganache
7. change 'ETH Admin' private key to the ganache first key
8. save the work and connect the account with with localhost:4200
(it wont work if you connect metamask with different tabs)
9. open another cmd and type truffle migrate to activate contracts migrations and roles
10. type truffle deploy
11. head back to localhost:4200 and click on admin
12. here is the dashboard of EHR Project

# FAQ
Q1: What if I want to open this project on Mac?

Mac users can try to prepare a VirtualBox Windows 10 virtual machine or equivalant. Windows Activation is not mandatory. With this virtual machine, Mac users can follow the steps above to open the project.

Q2: Why I cannot add doctor?

Due to a reported issue at github (https://github.com/shamil-t/ehr-blockchain/issues/15), a proper IPFS config is required to perform this feature properly. Check the installation section, step 1, to make sure your IPFS config ia set up correctly.
