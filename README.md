# Glass Billing System

A comprehensive billing and inventory management system for glass businesses, built with Next.js, Prisma, and MongoDB.

## Features

- Customer management
- Product catalog with pricing
- Invoice generation and management
- Payment tracking
- Tax calculation (SGST/CGST and IGST)
- Reports and analytics
- Bank account management
- Company profile management

## Setup Instructions

### Prerequisites

- Node.js 18+ installed
- MongoDB database (local or MongoDB Atlas)

### Installation

1. Clone the repository

```bash
git clone <repository-url>
cd glass-billing-system
```

2. Install dependencies

```bash
npm install
```

3. Set up environment variables

```bash
node scripts/setup-env.js
```

Follow the prompts to enter your MongoDB connection string.

4. Initialize the database

```bash
npx prisma db push
```

5. Start the development server

```bash
npm run dev
```

6. Open [http://localhost:3000](http://localhost:3000) in your browser

## Usage

1. Add your company information in the Settings page
2. Add your bank account details
3. Add products to your catalog
4. Add customers
5. Create invoices for your customers
6. Track payments
7. Generate reports

## Database Schema

The application uses MongoDB with Prisma ORM. The schema includes the following models:

- User: Authentication and user management
- Customer: Customer information
- Product: Product catalog with pricing
- Invoice: Invoice details with customer reference
- InvoiceItem: Line items for invoices
- Payment: Payment records for invoices
- BankAccount: Bank account information
- CompanyInfo: Company profile details

## Technology Stack

- **Frontend**: Next.js, React, Tailwind CSS, shadcn/ui
- **Backend**: Next.js API Routes
- **Database**: MongoDB with Prisma ORM
- **Authentication**: NextAuth.js
- **Charts**: Chart.js
- **PDF Generation**: Puppeteer
