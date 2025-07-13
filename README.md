# 📈 StockVault

**StockVault** is a modern, full-featured web application designed for simulated stock trading, portfolio management, and financial education. It provides an intuitive and responsive user interface along with powerful tools tailored for both beginner investors and experienced traders.

---

## 🚀 Key Features

- **User & Admin Authentication**  
  Secure registration, login, and session-based authentication with bcrypt password hashing.

- **Intuitive Dashboard**  
  Personalized user dashboard with portfolio summary, top performers, and motivational trading tips.

- **Stock Market Simulation**  
  Simulate stock trading with real-time price updates, search, and trading functionality.

- **Portfolio Management**  
  Track your holdings, profit/loss, and performance at a glance.

- **Integrated Wallet**  
  Deposit, withdraw, and view balances with complete transaction management.

- **Transaction History**  
  View a full log of all stock trades, deposits, and withdrawals.

- **Trading Glossary**  
  Built-in modal-based glossary for quick reference of trading terms and concepts.

- **Profile Management**  
  Update personal details and upload a profile picture.

- **Admin Panel**  
  A dedicated admin dashboard to manage users, stock data, and platform activity.

- **Responsive UI**  
  Seamlessly works across desktop, tablet, and mobile devices.

- **Polished UX Design**  
  Includes modals, animated login screens, tooltips, clean navigation, and modern UI components.

---

## 🛠️ Technology Stack

- **Frontend**: HTML, CSS, JavaScript, EJS Templates  
- **Backend**: Node.js, Express.js  
- **Database**: MySQL (schemas in `db/schema.sql`)  
- **Authentication**: Session-based with `bcrypt` for password hashing  
- **File Uploads**: Handled using Multer (profile pictures)  
- **Libraries**: FontAwesome, Chart.js  

---

## 📁 Project Structure

```
StockVault/
├── app.js                  # Main application file
├── db.js                   # Database connection
├── db/                     # SQL schema and setup scripts
│   ├── schema.sql
│   ├── create_tables.sql
│   └── admin_schema.sql
├── public/                 # Static assets
│   ├── css/                # style.css, admin.css
│   ├── img/                # Branding/media
│   ├── js/                 # main.js
│   └── uploads/profile/    # User profile pictures
├── routes/                 # Express route handlers
│   ├── admin.js
│   ├── auth.js
│   ├── portfolio.js
│   ├── profile.js
│   ├── stocks.js
│   ├── transactions.js
│   └── wallet.js
├── views/                  # EJS templates
│   ├── admin/              # Admin panel views
│   ├── auth/               # Login/register
│   ├── layouts/            # Master layouts
│   ├── partials/           # Header/footer
│   ├── portfolio/
│   ├── profile/
│   ├── stocks/
│   ├── transactions/
│   └── wallet/
├── package.json            # Project dependencies and scripts
└── README.md               # Project documentation
```

---

## ⚙️ Setup & Installation

### Prerequisites
- Node.js (v14 or higher)
- MySQL (v5.7 or higher)

### 1. Clone the Repository
```bash
git clone <your-repo-url>
cd TradePro
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure Environment Variables  
Create a `.env` file in the root directory:

```
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=yourpassword
DB_NAME=trading_new
SESSION_SECRET=your_secret_key
PORT=3000
```

### 4. Set Up the Database
- Create a MySQL database named `trading_new`
- Execute the SQL script in `db/schema.sql` to set up the tables and seed data.

### 5. Create Uploads Directory
```bash
mkdir -p public/uploads/profile
```

### 6. Start the Application
```bash
npm start
```

Visit [http://localhost:3000](http://localhost:3000) in your browser.

---

## 👥 User & Admin Workflows

- **User Flow**  
  Register → Login → Access Dashboard → Trade Stocks → Manage Portfolio, Wallet, and Profile.

- **Admin Flow**  
  Click “Test Admin Login” on the login screen to enter the admin dashboard and manage users and stock listings.

---

## 💡 UX Highlights

- Animated login screen with tabs for User/Admin access  
- Personalized dashboard greetings and random trading tips  
- In-app trading glossary for learning terms  
- Responsive layout with mobile-first design  
- Context-aware UI: shows/hides links and buttons based on user role  
- Fully functional—no broken or placeholder elements

---

## 📄 License

This project is intended for educational and demo purposes only.  
You’re welcome to use, modify, or extend it for personal learning or non-commercial use.
