# NextJS NFT Marketplace


## 1. Git clone the contracts repo

In it's own terminal / command line, run: 

```
git clone https://github.com/kaviraj-j/hardhat-nft-marketplace
cd hardhat-nextjs-nft-marketplace-fcc
yarn
```

## 2. Deploy to sepolia 

After installing dependencies, deploy your contracts to sepolia:

```
yarn hardhat deploy --network sepolia
```

## 3. Deploy your subgraph

```
cd ..
git clone https://github.com/kaviraj-j/graph-nft-marketplace-fcc
cd graph-nft-marketplace-fcc
yarn
```


Follow the instructions of the Patric Collin's Tutorial [README](https://github.com/PatrickAlphaC/graph-nft-marketplace-fcc/blob/main/README.md) of that repo. 

Then, make a `.env` file and place your temporary query URL into it as `NEXT_PUBLIC_SUBGRAPH_URL`.


## 4. Start your UI

Now clone this git repo

```
git clone https://github.com/kaviraj-j/nextjs-nft-marketplace
cd nextjs-nft-marketplace
```

Make sure that:
- In your `networkMapping.json` you have an entry for `NftMarketplace` on the sepolia network. 
- You have a `NEXT_PUBLIC_SUBGRAPH_URL` in your `.env` file.

```
yarn dev
```

