# CryptoPay Dashboard

CryptoPay is a **Web3-powered B2B dashboard** built with the **MERN stack** (MongoDB, Express, React, Node) and **TypeScript**.  
It allows users to connect their crypto wallet (e.g. MetaMask), view their Ethereum balance, send transactions, and log transaction history — all from a clean Tailwind-based admin dashboard.

----

## Features

- **Wallet Connection** — Connect MetaMask wallet via `ethers.js`
- **Live Balance Display** — Fetch real-time ETH balance
- **Send ETH** — Transfer ETH between wallets (real or testnet)
- **Transaction Logs** — Store and view transaction history in MongoDB
- **Admin Dashboard UI** — Built with Tailwind CSS for a responsive, modern look
- **Full MERN Stack** — React frontend + Node/Express backend + MongoDB storage
- **Environment-based Configuration** — Easily switch between testnet/mainnet

---

## Tech Stack

| Layer | Technology |
|-------|-------------|
| **Frontend** | React (Vite + TypeScript) |
| **Styling** | Tailwind CSS + Custom Admin Dashboard |
| **Blockchain** | ethers.js (MetaMask integration) |
| **Backend** | Node.js + Express.js |
| **Database** | MongoDB (Mongoose ORM) |
| **API** | RESTful JSON API |
| **Build Tool** | Vite |
| **Version Control** | Git + GitHub |

---

## 📂 Project Structure
```bash 
    cryptopay/
    ├── client/ # Frontend (React + TypeScript + Tailwind)
    │ ├── src/
    │ │ ├── components/ # Reusable components (WalletConnect, TransactionForm, etc.)
    │ │ ├── layout/ # Dashboard layout (sidebar, header, etc.)
    │ │ ├── pages/ # Dashboard pages
    │ │ ├── App.tsx
    │ │ └── main.tsx
    │ ├── index.html
    │ └── package.json
    │
    └── server/ # Backend (Express + MongoDB)
    ├── src/
    │ ├── models/ # Mongoose models
    │ ├── routes/ # Express routes
    │ ├── controllers/ # Business logic
    │ └── server.js
    ├── .env
    └── package.json
```

## Setup Instructions

### 1. Clone the repository

```bash
    git clone https://github.com/theo-georgewill/cryptopay.git
    cd cryptopay
```
### 2. Install dependencies

### Backend:
```bash 
    cd server
    npm install
```

### Frontend:
```bash
    cd ../client
    npm install
```

### 3. Setup environment variables
### /server/.env
```ini
    MONGO_URI=your_mongodb_connection_string
    PORT=5000
```

### /client/.env
```ini 
    VITE_API_BASE_URL=http://localhost:5000
```

## 4. Run the development servers
## Backend:

```bash 
cd server
npm run dev
```

### Frontend:

```bash 
cd ../client
npm run dev
```

### Core Components

| Component              | Description                               |
| ---------------------- | ----------------------------------------- |
| **WalletConnect**      | Connects MetaMask wallet via `ethers.js`  |
| **BalanceCard**        | Displays ETH balance                      |
| **TransactionForm**    | Send ETH to another wallet                |
| **TransactionHistory** | Displays saved transactions from MongoDB  |
| **Layout**             | Main dashboard layout (sidebar + content) |


### Future Enhancements

1. Multi-chain support (Polygon, BSC, etc.)
2. Token transfers (ERC20)
3. User authentication (JWT)
4. Analytics dashboard for transactions
5. Business accounts with spending limits

### Developer

Author: Theo Georgewill
Stack: MERN + Web3 + TypeScript
Email: ttggwll@gmail.com