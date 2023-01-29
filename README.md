# blockchainForHealthcare20221001

# Prerequisite
1. Windows 10 machine or virtual machine (Processors: All CPUs)
2. Google Chrome
3. Git
4. Node.js
5. Yarn (Use cmd to run this code to install: npm install --global yarn)
5. Truffle (Use cmd to run this code to install: npm install -g truffle)
5. Already following the videos in this playlist, from part 1 to part 7

https://www.youtube.com/playlist?list=PL54V-i7zW55d1VKxEkp9DCPt5k_zE6m3X

After following the videos, your pc should already have:

i. Ganache

ii. Google Chrome with Metamask

6. IPFS Desktop
7. Github Desktop

# Installation (Youtube: https://www.youtube.com/watch?v=1NuScL3KPKQ)
0. Make sure you meet the prerequisites
1. Open IPFS Desktop app and Change IPFS Settings

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

https://github.com/Nksheng/blockchainForHealthcare20221001

3. Turn on Ganache and make sure your ehr project is running. Add the new repo to Ganache.
4. Open your browser, and make sure MetaMask extension is logged in.
5. Go to metamask
6. Add 'ETH Admin' account with ganache first private key
7. Open cmd from this 'repo/Blockchain For Healthcare 20221001' folder
8. Type yarn install
9. Type yarn start
10. After that, press Ctrl+C to stop the project.
11. Check if Ganache still works properly. If has any issue, restart Ganache by following the dialog.
12. Type truffle migrate to activate contracts migrations and roles
13. Type truffle deploy
14. Type yarn start
15. In the browser, go to localhost:4200 and click on admin
16. here is the dashboard of EHR Project

# FAQ
Q1: What if I want to open this project on Mac?

Mac users can try to prepare a VirtualBox Windows 10 virtual machine or equivalant. Windows Activation is not mandatory. With this virtual machine, Mac users can follow the steps above to open the project.

Q2: Why I cannot add doctor?

Due to a reported issue at github (https://github.com/shamil-t/ehr-blockchain/issues/15), a proper IPFS config is required to perform this feature properly. Check the installation section, step 1, to make sure your IPFS config ia set up correctly.

Q3: Why the virtual machine need to access all CPUs?

Node.js will not function properly and can produce error like assertion time error if not all CPUs are used. To reduce the chance of the assertion time error, the virtual machine have to access all CPUs to run properly. Before a yarn command is run, make sure the clock is sync by checking FAQ Q4.

Q4: Assertion failed when yarn install, what should I do?

Go to Windows settings, Time & Language, Date & time. Then sync the time again by click Sync Now button under Synchronise the clock.