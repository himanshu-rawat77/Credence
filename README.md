# Credence - Decentralized Invoice Financing Platform

[![Demo Video](https://img.shields.io/badge/Demo-Watch%20Video-red?style=for-the-badge&logo=youtube)](https://youtu.be/TlZeikojPnw)
[![Next.js](https://img.shields.io/badge/Next.js-15.5.3-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![Node.js](https://img.shields.io/badge/Node.js-Express-green?style=for-the-badge&logo=node.js)](https://nodejs.org/)
[![MongoDB](https://img.shields.io/badge/MongoDB-Database-green?style=for-the-badge&logo=mongodb)](https://mongodb.com/)

## 🚀 Executive Summary

**Credence** is a revolutionary decentralized marketplace for invoice financing that transforms traditional receivables into programmable financial assets. Built on modern web technologies, Credence bridges the gap between real-world trade and digital liquidity, enabling businesses to unlock immediate working capital while providing financiers with transparent, secure investment opportunities.

## 🎯 The Problem We Solve

### For Businesses (SMEs)
- **Cash Flow Bottlenecks**: 30-120 day payment cycles create liquidity constraints
- **Limited Access**: Traditional banks offer slow, bureaucratic financing solutions
- **Opaque Pricing**: Hidden fees and unclear risk assessments
- **Credit Barriers**: Smaller businesses struggle with limited credit history

### For Financiers
- **Limited Asset Classes**: Few transparent ways to access receivables as investments
- **Lack of Liquidity**: Trillions in trade receivables remain locked and unproductive
- **Centralized Systems**: Traditional financing lacks transparency and efficiency

## 💡 Our Solution

Credence introduces a **Web3-native model** for invoice financing that combines trustless infrastructure with real-world trade:

### 🔗 Core Features

#### 1. **Invoice Tokenization**
- **NFT Route**: Each invoice as a unique NFT with embedded metadata
- **Token-2022 Route**: Fungible tokens supporting partial payments and programmable transfers
- **Decentralized Storage**: Secure invoice data on Arweave/IPFS

#### 2. **Decentralized Bidding Marketplace**
- **Competitive Pricing**: Banks and investors compete for financing opportunities
- **Transparent Process**: All bids and transactions recorded on-chain
- **Fair Access**: Open marketplace ensures equal opportunities

#### 3. **Smart Escrow Contracts**
- **Automated Payments**: Programmable escrow accounts handle repayments
- **Secure Distribution**: Guaranteed financier payouts before invoice settlement
- **Trustless Operations**: No intermediaries required

#### 4. **Transparent Lifecycle Management**
- **On-Chain Records**: Every step from issuance to repayment tracked
- **Real-time Updates**: Live status updates for all stakeholders
- **Audit Trail**: Complete transaction history for compliance

## 🏗️ Technical Architecture

### Frontend (Next.js 15.5.3)
- **Modern React**: Built with React 19.1.0 and TypeScript
- **Responsive Design**: Mobile-first approach with Tailwind CSS
- **Real-time Updates**: Live marketplace and bidding interface
- **Role-based Access**: Separate interfaces for Organizations, Financiers, and Customers

### Backend (Node.js + Express)
- **RESTful API**: Comprehensive API with proper error handling
- **Authentication**: JWT-based security with role-based access control
- **Rate Limiting**: Protection against abuse and spam
- **Logging**: Comprehensive logging with Winston
- **Security**: Helmet, CORS, and input sanitization

### Database (MongoDB)
- **Scalable Schema**: Optimized for invoice and user management
- **Indexing**: Performance-optimized queries
- **Relationships**: Proper data modeling for complex relationships

## 🎭 User Roles & Workflows

### 🏢 Organizations (Sellers)
1. **Create Invoices**: Generate professional invoices with line items
2. **List on Marketplace**: Submit invoices for financing
3. **Accept Bids**: Choose the best financing offer
4. **Receive Funds**: Get 80-90% upfront liquidity
5. **Track Status**: Monitor invoice lifecycle and payments

### 💰 Financiers (Investors)
1. **Browse Marketplace**: View available invoice listings
2. **Place Bids**: Competitive bidding on preferred invoices
3. **Manage Portfolio**: Track investments and returns
4. **Receive Payments**: Automated payouts when customers pay
5. **Risk Assessment**: Access customer credit information

### 👥 Customers (Buyers)
1. **View Invoices**: Access detailed invoice information
2. **Make Payments**: Secure payment processing
3. **Track History**: Complete payment and invoice history
4. **Notifications**: Real-time updates on invoice status

## 🚀 Key Features

### For Organizations
- ✅ **Professional Invoice Creation** with customizable templates
- ✅ **Automated Calculations** for taxes, discounts, and totals
- ✅ **Marketplace Integration** for instant liquidity
- ✅ **Real-time Analytics** and reporting
- ✅ **Customer Management** with payment tracking
- ✅ **Notification System** for payment reminders

### For Financiers
- ✅ **Investment Dashboard** with portfolio overview
- ✅ **Competitive Bidding** system
- ✅ **Risk Assessment Tools** with customer data
- ✅ **Automated Returns** when invoices are paid
- ✅ **Balance Management** with locked/unlocked funds
- ✅ **Market Analytics** for informed decisions

### For Customers
- ✅ **Invoice Portal** with detailed breakdowns
- ✅ **Secure Payment Processing** with multiple options
- ✅ **Payment History** and receipts
- ✅ **Real-time Notifications** for due dates
- ✅ **Mobile-responsive** interface

## 🛠️ Installation & Setup

### Prerequisites
- Node.js 18+ 
- MongoDB 6+
- npm or yarn

### Backend Setup
```bash
cd backend
npm install
cp config.env.example config.env
# Configure your environment variables
npm run dev
```

### Frontend Setup
```bash
npm install
npm run dev
```

### Environment Variables
Create a `backend/config.env` file with:
```env
NODE_ENV=development
PORT=5000
MONGODB_URI=mongodb://localhost:27017/credence
JWT_SECRET=your_jwt_secret
JWT_EXPIRES_IN=90d
EMAIL_USERNAME=your_email
EMAIL_PASSWORD=your_password
```

## 📊 API Endpoints

### Authentication
- `POST /api/v1/auth/register` - User registration
- `POST /api/v1/auth/login` - User login
- `POST /api/v1/auth/logout` - User logout

### Organizations
- `GET /api/v1/organizations` - Get organization profile
- `POST /api/v1/organizations` - Create organization
- `PUT /api/v1/organizations` - Update organization

### Invoices
- `GET /api/v1/invoices` - List invoices
- `POST /api/v1/invoices` - Create invoice
- `GET /api/v1/invoices/:id` - Get invoice details
- `PUT /api/v1/invoices/:id` - Update invoice

### Marketplace
- `GET /api/v1/marketplace` - List marketplace items
- `POST /api/v1/marketplace` - Create listing
- `POST /api/v1/marketplace/:id/bid` - Place bid
- `DELETE /api/v1/marketplace/:id/bid/:bidId` - Cancel bid

### Financiers
- `GET /api/v1/financiers` - Get financier profile
- `POST /api/v1/financiers` - Create financier
- `POST /api/v1/financiers/balance` - Add balance

## 🔒 Security Features

- **JWT Authentication** with role-based access control
- **Rate Limiting** to prevent abuse
- **Input Validation** and sanitization
- **CORS Protection** for cross-origin requests
- **Helmet Security** headers
- **XSS Protection** with input cleaning
- **MongoDB Injection** prevention

## 📈 Competitive Advantages

### 🎯 **Decentralized & Transparent**
- No intermediaries or hidden fees
- All transactions recorded on-chain
- Open-source and auditable

### 💧 **Liquidity Unlocking**
- SMEs get immediate cash flow (80-90% upfront)
- No more waiting 30-120 days for payments
- Flexible financing terms

### 🏦 **New Asset Class**
- Trade receivables become investable
- Liquid and transferable assets
- Composable with DeFi protocols

### ⚡ **Low-Cost & Scalable**
- Efficient transaction processing
- Minimal fees compared to traditional banking
- Global accessibility

## 🌍 Use Cases

### **SMEs** needing immediate liquidity against invoices
### **Banks** diversifying into receivable-backed lending
### **DeFi Investors** seeking safe, real-world yield opportunities
### **Cross-border Trade** financing in underserved regions

## 🎥 Demo & Documentation

- **📺 [Watch Demo Video](https://youtu.be/TlZeikojPnw)** - See Credence in action
- **📚 API Documentation** - Comprehensive endpoint documentation
- **🔧 Developer Guide** - Setup and integration instructions

## 🚀 Getting Started

1. **Clone the repository**
2. **Set up your environment** (MongoDB, Node.js)
3. **Install dependencies** (`npm install`)
4. **Configure environment variables**
5. **Run the application** (`npm run dev`)
6. **Access the platform** at `http://localhost:3000`

## 🤝 Contributing

We welcome contributions! Please see our contributing guidelines for:
- Code style and standards
- Pull request process
- Issue reporting
- Feature requests

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

## 🔮 Vision

**"Turn invoices into programmable money"**

Just as the Finternet aspires to create a single, open financial system, Credence bridges real-world receivables into internet-native capital markets. We envision a future where:

- ✅ No business waits 120 days to get paid
- ✅ Financiers worldwide access receivable-backed assets seamlessly
- ✅ Transparent, borderless marketplace for trade financing
- ✅ Credence becomes the liquidity base layer for global trade

---

**Credence** - *Connecting businesses, banks, and DeFi into one seamless system.*

[![Demo Video](https://img.shields.io/badge/Demo-Watch%20Video-red?style=for-the-badge&logo=youtube)](https://youtu.be/TlZeikojPnw)