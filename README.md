# AnkitPunks NFT DAO
🔨 Building our DAO

We want to launch a DAO for holders of our NFT Collection - AnkitPunks. From the ETH that was gained through the sale of the NFTs, we have built up a treasury. The DAO now has a lot of ETH, but currently does nothing with it.

We want to allow our NFT holders to create and vote on proposals to use that ETH for purchasing other NFTs from an NFT marketplace, and speculate on price. Maybe in the future when we sell the NFT back, we may split the profits among all members of the DAO.

📝 Requirements

Anyone who owns a AnkitPunks NFT can create a proposal to purchase a different NFT from an NFT marketplace

Everyone with a AnkitPunks NFT can vote for or against the active proposals

Each NFT counts as one vote for each proposal

Voters cannot vote multiple times on the same proposal with the same NFT

If majority of the voters vote in favor of the proposal by the deadline, the NFT purchase happens automatically from the marketplace

🔩 What we will make

First, we will create a basic NFT contract for the AnkitPunks collection so we have something to test with.

Second, for the DAO to be able to purchase NFTs automatically on-chain when a proposal is passed, we need to use an on-chain NFT marketplace. While there exist a lot of on-chain NFT Marketplaces such as Seaport by OpenSea - we will create our own fake little NFT Marketplace that simulates the behavior of a real one to keep things simple and not turn this into a lesson about understanding the Seaport codebase.

Third, we will write a custom smart contract for the DAO itself where proposals can be created, voted upon, and executed on-chain.

Lastly, we will build a simple website using Next.js to allow users to create and vote on proposals.

Try running some of the following tasks:

```shell
npm init --yes
npm install --save-dev hardhat @nomicfoundation/hardhat-toolbox
npx hardhat
npm install @openzeppelin/contracts
npm install dotenv
npx hardhat run scripts/deploy.js --network sepolia
npx create-next-app@12
npm install @rainbow-me/rainbowkit wagmi viem
npm run dev
```
