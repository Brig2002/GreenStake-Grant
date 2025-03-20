
# GreenStake - Decentralized Project Funding Platform

GreenStake is a decentralized platform that enables transparent and community-driven project funding through a DAO (Decentralized Autonomous Organization) governance model. Built on the Arbitrum Sepolia network, it allows project creators to list their initiatives and receive donations while ensuring proper oversight through DAO member voting.

## Features

### For Project Creators
- **Project Listing**: List your project with a name and description
- **Subscription-based**: 30-day active listing period
- **Transparent Funding**: Receive 80% of all donations directly
- **Community Approval**: Get validated by DAO members

### For DAO Members
- **Governance Rights**: Vote on project approvals
- **Staking Mechanism**: Join by staking 0.01 ETH
- **Revenue Share**: Earn 15% of project donations split among members
- **Community Power**: Influence platform direction

### For Donors
- **Direct Support**: Donate to approved projects
- **Transparent Distribution**:
  - 80% to project owner
  - 15% to DAO members
  - 5% platform fee

## Technical Architecture

### Smart Contracts
1. **ProjectListing.sol**
   - Manages project listings
   - Handles subscription fees
   - Tracks project status and donations

2. **DAO.sol**
   - Manages DAO membership
   - Handles project voting
   - Distributes member rewards

3. **Donate.sol**
   - Processes donations
   - Manages fund distribution
   - Tracks donation history

### Frontend
- Built with Next.js and Wagmi
- Real-time blockchain interaction
- Responsive and user-friendly interface

## Getting Started

### Prerequisites
- Node.js v16 or higher
- MetaMask wallet
- Some Arbitrum Sepolia ETH for transactions

### Installation

1. Clone the repository
```bash
git clone https://github.com/Brig2002/GreenStake-Grant.git
cd Apetorku
```

2. Install dependencies
```bash
# Install contract dependencies
cd GreenStake-Contract
npm install

# Install frontend dependencies
cd ../frontend
npm install
```

3. Set up environment variables
```bash
# In GreenStake-Contract/.env
PRIVATE_KEY=your_private_key
ARBITRUM_SEPOLIA_RPC_URL=your_rpc_url
```

4. Deploy contracts
```bash
cd GreenStake-Contract
npx hardhat run scripts/deploy.js --network arbitrumSepolia
```

5. Start the frontend
```bash
cd ../frontend
npm run dev
```

## Usage

### For Project Creators
1. Connect your wallet
2. Click "List Project"
3. Pay 0.01 ETH listing fee
4. Wait for DAO approval

### For DAO Members
1. Connect your wallet
2. Click "Join DAO"
3. Stake 0.01 ETH
4. Vote on projects

### For Donors
1. Connect your wallet
2. Browse approved projects
3. Click "Donate" on your chosen project
4. Confirm transaction

## Contract Addresses (Arbitrum Sepolia)

- ProjectListing: [Latest Deployed Address]
- DAO: [Latest Deployed Address]
- Donate: [Latest Deployed Address]

## Security Considerations

- ReentrancyGuard implemented on all contracts
- Proper access control using Ownable
- Safe math operations with Solidity 0.8+
- Thorough input validation
- Secure fund distribution

## Contributing

1. Fork the repository
2. Create your feature branch
3. Commit your changes
4. Push to the branch
5. Create a new Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- OpenZeppelin for secure contract implementations
- Hardhat for development framework
- Next.js for frontend framework
- Wagmi for Web3 hooks
