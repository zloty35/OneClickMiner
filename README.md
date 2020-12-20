# OneClickMiner
Simple blockstack miner - even muggle can run it!

Before you start:
1. Create a Testnet STX & BTC Address -> you can check YT tutorial https://www.youtube.com/watch?v=82b8PGoQYpI&feature=youtu.be&ab_channel=Freehold
2. Top up some BTC to your testnet BTC address, you can use powershell request listed at the bottom of this file
3. The miner works on Windows 10 x64


How to run the miner:
1. Unzip OneClickMiner.zip
2. Paste your BTC (testnet) private key into config.toml - seed field
3. Run StartMiner
4. Thats all, you run the miner.


How to ensure your miner actually works:
Go to your web browser and open below two sites
http://krypton.blockstack.org:20443/v2/info
http://localhost:20443/v2/info
The result has to be equal except operating system. Blockstack runs Linux, your is Windows.
Please note that result is different until your miner is fully synced - usually it takes 30 min.



Useful Powershell commands powershell is available on each Windows, search for Windows PowerShell.

#Request BTC(testnet)
Invoke-WebRequest -Method POST -Body (@{"address"="YOUR_BTC_ADDRESS";}) -Uri https://stacks-node-api.krypton.blockstack.org/extended/v1/faucets/btc

#Check BTC(testnet) balance
Invoke-WebRequest -Uri https://stacks-node-api.krypton.blockstack.org/extended/v1/faucets/btc/TWOJ_ADRES_tBTC

#Check STX(testnet) balance
Invoke-WebRequest -Uri https://stacks-node-api.krypton.blockstack.org/extended/v1/address/TWOJ_ADRES_STX/stx


Regards,
zloty35

