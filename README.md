# WalletKit Demo Project

A demo wallet interface showcasing the integration of Reown [WalletKit](https://docs.reown.com/walletkit/web/usage) with Next.js. This wallet is live at [https://walletkit-reown.vercel.app/](https://walletkit-reown.vercel.app/).

## Demo 

https://github.com/user-attachments/assets/8c46590d-ab9e-4488-a46d-0d12a312da18

## Prerequisites

Before you begin, ensure you have the following installed:
- Node.js (version 16 or higher)
- Ngrok or similar tunneling service (for HTTPS access)

## Setup

1. Clone the repository:

```bash
git clone https://github.com/walletkit/walletkit-demo.git
```

2. Install dependencies:

```bash
pnpm install
```

3. Environment Setup:

Copy the `.example.env` file to `.env.local`:

```bash
cp .example.env .env.local
```

- Update the environment variables in `.env.local`:
  - `NEXT_PUBLIC_PROJECT_ID`: Your WalletConnect Project ID (required)
  - `NEXT_PUBLIC_PRIVATE_KEY`: Your private key (optional)

## Running the Project

1. Start the development server:

```bash
pnpm dev
```

2. Start ngrok or similar tunneling service:

```bash
ngrok http 3000 // replace 3000 with the port number of your local server
```

3. Use the HTTPS URL provided by ngrok to access your application

## Project Structure

- `/src/app`: Main application pages and layouts
- `/src/components`: Reusable UI components
- `/src/context`: React context providers
- `/src/hooks`: Custom React hooks
- `/src/utils`: Utility functions
- `/src/store`: State management using Zustand
- `/src/types`: TypeScript type definitions

## Features

- Connect with any dApp that supports WalletConnect
- Session management, with the ability to connect, accept, reject, and delete sessions
- Message signing, sign messages with your wallet from any connected dApp



