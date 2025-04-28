# Smart Contract Counter

A decentralized counter application built with sCrypt and React, demonstrating basic smart contract functionality on the Bitcoin SV blockchain.

## Features

- Smart contract-based counter implementation
- Real-time counter updates
- Secure private key management
- Modern React frontend
- TypeScript support

## Prerequisites

- Node.js (v14 or higher)
- pnpm
- Git
- Bitcoin SV wallet with testnet funds

## Getting Started

1. Clone the repository:
```bash
git clone <repository-url>
cd sc-counter
```

2. Install dependencies:
```bash
pnpm install
```

3. Set up your environment variables:
   - Copy the sample environment file:
     ```bash
     cp src/env.sample.tsx src/env.tsx
     ```
   - Open `src/env.tsx` and replace `'YOUR_PRIVATE_KEY_HERE'` with your actual private key
   - Note: Never commit your `env.tsx` file to version control

4. Compile the smart contract:
```bash
npx scrypt-cli@latest compile
```

5. Start the development server:
```bash
pnpm start
```

The application will be available at [http://localhost:3000](http://localhost:3000).

## Project Structure

```
sc-counter/
├── src/
│   ├── components/     # React components
│   ├── contracts/      # sCrypt smart contracts
│   ├── env.tsx        # Environment variables (gitignored)
│   └── env.sample.tsx # Environment template
├── public/            # Static assets
└── tests/            # Test files
```

## Available Scripts

### `pnpm start`
Runs the app in development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

### `pnpm test`
Launches the test runner in interactive watch mode.

### `pnpm run build`
Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

## Smart Contract

The counter smart contract is implemented in sCrypt and provides the following functionality:
- Increment counter
- Decrement counter
- Get current counter value

## Security Considerations

- Never commit your private keys to version control
- Always use testnet for development
- Keep your `env.tsx` file secure and local
- Review smart contract code before deployment

## Learn More

- [sCrypt Documentation](https://scrypt.io/docs/)
- [React Documentation](https://reactjs.org/)
- [Bitcoin SV Documentation](https://docs.bitcoinsv.io/)

## License

This project is licensed under the MIT License - see the LICENSE file for details.
