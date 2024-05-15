# Catalyst-tuto
Catalyst Node project on Mobaxterm

🔍PROCESSEUR AMD ex : CPX31  "Hetzner Website"
_________________________________________________________________________ 
💻 Write on Mobaxterm : 

sudo apt update && sudo apt upgrade -y 

sudo apt-get update 

sudo apt-get install \ 
 ca-certificates \ 
 curl \ 
 gnupg \ 
 lsb-release 

curl -fsSL https://download.docker.com/linux/ubuntu/gpg | sudo gpg --dearmor -o 
/usr/share/keyrings/docker-archive-keyring.gpg 

echo \ 
 "deb [arch=$(dpkg --print-architecture) signed-by=/usr/share/keyrings/docker-archive￾keyring.gpg] https://download.docker.com/linux/ubuntu \ 
 $(lsb_release -cs) stable" | sudo tee /etc/apt/sources.list.d/docker.list > /dev/null 

sudo apt-get update 

docker compose version 

sudo apt-get install docker-ce docker-ce-cli containerd.io docker-buildx-plugin docker-compose￾plugin 

git clone https://github.com/catalystdao/generalised-relayer.git 
cd generalised-relayer 

cp config.example.yaml config.production.yaml 
cp .env.example .env 

vim config.production.yaml

📁 Create a wallet and export the private key, add "0x" at the beginning of it.

export NODE_ENV=production 

echo "export NODE_ENV=production" >> ~/.bashrc 

docker compose up -d 

docker compose logs relayer -fn 100 

cd .. 

git clone https://github.com/catalystdao/catalyst-underwriter.git 
cd catalyst-underwriter 

cp config.example.yaml config.production.yaml 
cp .env.example .env

📁 Export the private key, add "0x" at the beginning of it.

docker compose up -d

📕 Check Underwriter : docker compose logs underwriter -fn 100

⚠️ Retrieve ETH Sepolia from the Alchemy faucet: https://www.alchemy.com/faucets/ethereum-sepolia, then on https://app.catalyst.exchange/ swap your ETH into WETH.

