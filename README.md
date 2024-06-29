## Unleash the Future of Gaming - Where Chainlink-powered NFTs, Fair Play, and Decentralized Finance Merge into Your Ultimate Web3 Gaming Hub.

Welcome to BetBlock, the revolutionary Web3 gaming platform that combines the thrill of gaming with the power of blockchain technology. BetBlock is designed to be your one-stop gaming hub, offering a seamless blend of gaming, social interaction, and decentralized finance (DeFi), all powered by Chainlink.

## Project Overview

BetBlock is inspired by the vision of a fully integrated Web3 gaming ecosystem. It leverages Chainlink's decentralized services to ensure fair play, create unique NFT-based identities, and facilitate cross-chain financial transactions. Our platform is akin to the PlayStation experience but built for the blockchain era, enabling players to connect, compete, and thrive in a decentralized gaming world.

### Key Features

- **Chainlink Functions:** Generative NFT Profile Creation acts a core piece for the community/social aspect of our product where every player will be able to mint their own NFT avatar using DALL-E3(Open AI). These functions is implemented in the mint logic where the smart contract will call our own API and self hosted IPFS Server to create AI generated images using input ket words for player NFT PFPs.(Can be seen in ProfileNFTContract.sol) 

- **Chainlink VRF:** Provably Fair Gaming was used to ensure transparency and fairness in our casino games. When a user places a bet, the smart contract makes a request to the Chainlink VRF to get a random number then the VRF returns a random number along with cryptographic proof of fair randomness. (Can be seen in Roulette.sol)

- **Chainlink Automation:** For rolutte contract, the player places all their bets on the board. Chainlink Automation is used to automatically spin the roulette wheel and calculate winnings once the place bet transaction has been recorded on chain. This ensures that there is always a result returned every time a bet is placed. (Can be seen in Roulette.sol)

- **Chainlink Data Feeds:** Access in-dApp DeFi lending services to borrow gaming assets without selling your holdings, you see multiple assets you can use as collateral for borrowing USDC. Chainlink Data Feeds is used to get accurate and relaible market price data. This is important to correctly calculate the collateralization factor and max LTV for each asset. (Can be seen in PolygonLending.sol)

- **Social Networking:** Connect with friends via ENS, compete for leaderboard rankings, and showcase your NFT achievements.

## Technology Stack

- **Smart Contracts:** Solidity, deployed on Polygon and Avalanche
- **Frontend:** React.js, Material UI, Three.js for 3D graphics, and Lottie for animations
- **Web3 Integration:** Viem for seamless blockchain interaction
- **Data Storage:** IPFS for decentralized storage of NFTs and metadata
- **Oracles:** Chainlink VRF, Chainlink Data Feeds, Chainlink Automation, and Chainlink Functions for on-chain randomness, asset prices, automated gameplay, and external data retrieval

## Getting Started

To start exploring BetBlock, follow these steps to set up the platform locally.

### Prerequisites

- Node.js
- Yarn
- Git
- A Web3 wallet (e.g., MetaMask)

### Setup

1. Clone the repository.
   
2. Install dependencies:
    ```bash
    cd betblock
    yarn install
    ```
3. Start the local development server:
    ```bash
    yarn start
    ```

### Smart Contract Deployment

Refer to the `betblock-contracts` README for detailed instructions on deploying the contracts to your preferred blockchain network.

## Acknowledgments

- Chainlink for their powerful decentralized oracle network
- OpenAI for the DALL-E API used in NFT generation
- The Web3 community for continuous inspiration and support

BetBlock is more than just a platform, it's a launchpad for games, a new way to game, and a glimpse into the future of decentralized entertainment.
