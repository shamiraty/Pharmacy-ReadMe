# PharmaCare Management System - User Manual

## Table of Contents
1. [Introduction](#introduction)
2. [Getting Started](#getting-started)
3. [System Features](#system-features)
4. [User Roles and Permissions](#user-roles-and-permissions)
5. [How to Use the System](#how-to-use-the-system)
6. [Understanding Reports and Analytics](#understanding-reports-and-analytics)
7. [Import and Export Data](#import-and-export-data)
8. [Technologies Used](#technologies-used)
9. [Installation Requirements](#installation-requirements)

---

## Introduction

PharmaCare is a complete pharmacy management system designed to help you efficiently manage your pharmacy operations. The system handles everything from medicine inventory to sales tracking, user management, and comprehensive reporting.

### What Can You Do With PharmaCare?

- **Manage Medicines**: Add, edit, and track your medicine inventory
- **Process Sales**: Quick point-of-sale system for customer transactions
- **Track Users**: Manage staff members and their access levels
- **Generate Reports**: Get detailed insights into your business performance
- **Monitor Stock**: Receive alerts for low stock and expiring medicines
- **Export Data**: Download reports in Excel, PDF, or Word formats
- **Import Medicines**: Bulk upload medicine data using CSV files

---

## Getting Started

### First Time Login

1. Open your web browser and go to: `http://localhost:3001/login`
2. Enter the default admin credentials:
   - **Email**: admin@pharmacy.com
   - **Password**: admin123
3. Click "Sign In"

**Important**: After your first login, we recommend changing the admin password for security.

### System Navigation

Once logged in, you'll see:

- **Top Bar**: Shows current time, date, and your user profile
- **Sidebar**: Main navigation menu with access to all features
- **Dashboard**: Your starting point showing today's statistics

---

## System Features

### 1. Dashboard

Your dashboard provides an overview of your pharmacy's performance:

- **Today's Statistics**: View sales count and revenue for the current day
- **Sales Trends**: 7-day chart showing your sales patterns
- **Top Selling Medicines**: See which products are most popular
- **Low Stock Alerts**: Get notified about medicines running low
- **Expiring Medicines**: Track medicines approaching expiry dates

### 2. Point of Sale (Sales)

This is where you process customer transactions:

**How to Make a Sale:**
1. Click "Sales" in the sidebar
2. Select medicines from the dropdown menu
3. Enter quantity for each item
4. Add customer name and phone (optional)
5. Choose payment method (Cash, Card, or M-Pesa)
6. Enter amount paid
7. Click "Complete Sale"
8. Print or download the invoice

**Features:**
- Real-time stock checking
- Automatic change calculation
- Multiple payment methods
- Instant invoice generation
- Sales history tracking

### 3. Medicines Management

Manage your complete medicine inventory:

**Medicine Information Includes:**
- Medicine name and generic name
- Category (Painkillers, Antibiotics, etc.)
- Stock quantity
- Purchase price (what you paid)
- Selling price (full and half units)
- Expiry date
- Manufacturer
- Storage location

**Actions Available:**
- View medicine details
- Add new medicines (Admin only)
- Edit medicine information (Admin only)
- Delete medicines (Admin only)
- Search and filter by category
- Export inventory lists

### 4. Inventory Tracking

Monitor your stock levels and sales history:

**What You Can See:**
- Current stock for each medicine
- Stock status (In Stock, Low Stock, Out of Stock)
- Total value of inventory
- Sales history for each medicine
- Who sold each item and when

**Stock Alerts:**
- Green: Plenty in stock (50+ units)
- Yellow: Low stock (10-49 units)
- Red: Out of stock (0-9 units)

### 5. Users Management

Control who can access your system (Admin only):

**User Information:**
- Full name
- Email address
- Role (Admin, Pharmacist, Cashier)
- Status (Active/Inactive)

**Actions:**
- Add new users
- Edit user details
- Change user roles
- Activate/deactivate accounts

### 6. Invoices

View and manage all sales invoices:

**Features:**
- Search invoices by number or customer name
- Filter by date range
- View invoice details
- Download individual invoices as PDF
- Track payment status

### 7. Purchase Management

Record and track medicine purchases:

**Purchase Details:**
- Supplier information
- Purchase date
- Medicine purchased
- Quantity and cost
- Total purchase amount

### 8. Analytics and Reports

Get detailed insights into your business:

**Medicine Analytics:**
- Sales performance by medicine
- Profit analysis
- Stock movement trends
- Category-wise breakdown

**Sales Analytics:**
- Daily, weekly, and monthly sales
- Revenue trends
- Payment method analysis
- Cashier performance
- Customer purchase patterns

**Available Filters:**
- Date range
- Payment method
- User/Cashier
- Customer name
- Medicine category

---

## User Roles and Permissions

### Admin (Full Access)
Administrators have complete control over the system:

✅ **Can Do Everything:**
- View all reports and statistics
- Make sales transactions
- Add, edit, and delete medicines
- Manage user accounts
- Import/export data
- Access all analytics
- Change system settings

### Cashier (Sales Staff)
Cashiers handle front-desk operations:

✅ **Can Do:**
- View dashboard
- Process sales
- View medicine inventory
- Search for medicines
- Generate invoices
- View sales history

❌ **Cannot Do:**
- Add or edit medicines
- Manage users
- Import medicines
- Change system settings

### Pharmacist (Future Feature)
Pharmacists will have permissions between Admin and Cashier:
- Make sales
- View and edit medicine details
- Manage inventory levels
- Access analytics
- Export reports

---

## How to Use the System

### Adding a New Medicine

1. Go to "Medicines" in the sidebar
2. Click "Add Medicine" button (Admin only)
3. Fill in the medicine details:
   - **Name**: Medicine brand name (e.g., "Panadol Extra")
   - **Generic Name**: Chemical name (e.g., "Paracetamol")
   - **Category**: Select category (e.g., "Painkillers")
   - **Purchase Price (Carton)**: Total cost you paid for a carton
   - **Units Per Carton**: How many individual units in the carton
   - **Selling Price (Full)**: Price for a full unit
   - **Selling Price (Half)**: Price for half unit (if applicable)
   - **Quantity in Stock**: Current stock count
   - **Expiry Date**: When the medicine expires
   - **Manufacturer**: Company name
   - **Location**: Storage location (e.g., "Shelf A3")
4. Click "Add Medicine"

**Understanding Pricing:**
- If you bought a carton for TZS 50,000 with 500 units inside
- Each unit costs you: 50,000 ÷ 500 = TZS 100
- If you sell each unit for TZS 500
- Your profit per unit: 500 - 100 = TZS 400

### Processing a Customer Sale

1. Click "Sales" in the sidebar
2. Select a medicine from the dropdown
3. Enter the quantity to sell
4. Click "Add to Cart"
5. Repeat for additional items
6. Enter customer details (optional but recommended):
   - Customer name
   - Phone number
7. Select payment method
8. Enter amount paid by customer
9. System shows change to give (if any)
10. Click "Complete Sale"
11. Choose to print or download the invoice

**Tips:**
- The system automatically checks stock availability
- You can remove items from cart before completing
- All sales are tracked with your user ID
- Invoices are automatically numbered

### Managing Users (Admin Only)

1. Go to "Users" in the sidebar
2. Click "Add User" button
3. Enter user details:
   - Full name
   - Email address (used for login)
   - Password (user will use this to login)
   - Role (Admin, Pharmacist, or Cashier)
4. Click "Add User"

**To Edit a User:**
1. Find the user in the list
2. Click the edit button (pencil icon)
3. Update the information
4. Click "Update User"

**To Deactivate a User:**
1. Find the user in the list
2. Click the delete button
3. Confirm the action

### Viewing Inventory Status

1. Click "Inventory" in the sidebar
2. View all medicines with their stock levels
3. Color-coded status shows:
   - **Green**: Good stock (50+ units)
   - **Yellow**: Low stock (10-49 units)
   - **Red**: Critical stock (0-9 units)

**To View Sales History:**
1. Click the eye icon next to any medicine
2. See complete sales history including:
   - When it was sold
   - Who sold it
   - Invoice number
   - Customer name
   - Quantity and price
3. Export this history to Excel or PDF if needed

---

## Understanding Reports and Analytics

### Reading the Dashboard

**Today's Statistics:**
- **Sales Count**: Number of transactions today
- **Revenue**: Total money received today
- These numbers update in real-time as you make sales

**7-Day Sales Trend:**
- Shows sales pattern over the past week
- Helps identify busy days
- Plan staff scheduling accordingly

**Top Selling Medicines:**
- Lists medicines by sales frequency
- Shows total revenue per medicine
- Calculated profit for each medicine
- Helps with reordering decisions

### Understanding Profit Calculations

**Example Scenario:**
- You bought a carton for TZS 50,000
- The carton contains 500 units
- Your cost per unit: 50,000 ÷ 500 = TZS 100
- You sell each unit for TZS 500
- You sold 10 units today

**Calculations:**
1. **Revenue**: 10 units × TZS 500 = TZS 5,000
2. **Cost**: 10 units × TZS 100 = TZS 1,000
3. **Profit**: TZS 5,000 - TZS 1,000 = TZS 4,000

**Stock Value:**
- Remaining stock: 90 units
- Stock value: 90 × TZS 100 = TZS 9,000
- This is your money "locked" in inventory

### Sales Analytics Reports

**Revenue Report:**
- Shows total money received
- Breaks down by payment method
- Groups by time period (daily, weekly, monthly)

**Top Medicines Report:**
- **Revenue**: Total sales amount
- **Profit**: Revenue minus cost
- **Frequency**: How many times sold (not quantity)
  - Frequency = 5 means 5 different customers bought it
  - This shows popularity, not quantity

**Transaction Report:**
- Lists all sales invoices
- Shows amount paid and change given
- Identifies any unpaid balances

---

## Import and Export Data

### Importing Medicines (Bulk Upload)

Save time by uploading multiple medicines at once using a CSV file.

**How to Import:**
1. Click "Medicines" in the sidebar
2. Click "Import" button (Admin only)
3. Choose your CSV file
4. System validates the data and shows preview
5. Review the preview:
   - Green checkmarks = valid data
   - Red marks = errors found
6. Click "Confirm Import" if everything looks good

**CSV File Format:**
Your CSV file must include these columns:
- `name` (required)
- `category` (required)
- `stock` (required - must be a number)
- `price_full` (required - selling price)
- `generic_name` (optional)
- `expiry_date` (optional - format: YYYY-MM-DD)
- `manufacturer` (optional)
- `price_half` (optional)

**Important Notes:**
- If a medicine with the same name exists, the stock will be added together
- Prices and other details will be updated to the new values
- If a medicine is new, it will be created

**Example CSV:**
```
name,category,stock,price_full,generic_name,manufacturer
Panadol Extra,Painkillers,100,500,Paracetamol,GSK
Amoxil 500mg,Antibiotics,50,1500,Amoxicillin,Pfizer
```

### Exporting Data

You can export data in three formats: Excel, PDF, and Word.

**Excel Export:**
- Best for further analysis
- Can be opened in Microsoft Excel or Google Sheets
- Includes multiple sheets with detailed breakdowns
- Preserves all data for calculations

**PDF Export:**
- Best for printing or sharing
- Professional report format
- Includes charts and tables
- Read-only format

**Word Export:**
- Good for editing reports
- Can add your own notes
- Professional document format

**What You Can Export:**
- Medicine inventory lists
- Sales reports
- Invoice copies
- Analytics reports
- Transaction history
- Medicine sales history

**How to Export:**
1. Go to the page you want to export (Medicines, Sales Analytics, etc.)
2. Click "Export" or "Export Report" button
3. Choose your preferred format (Excel, PDF, or Word)
4. File downloads automatically
5. Open with appropriate program

---

## Technologies Used

PharmaCare is built using modern, reliable technologies:

### Core Technologies

**1. Next.js (React Framework)**
- Powers the user interface
- Provides fast page loading
- Enables smooth navigation
- Version used: Latest stable release

**2. React.js**
- Creates interactive components
- Handles user interactions
- Manages data updates in real-time
- Makes the system responsive and fast

**3. SQLite Database**
- Stores all your data locally
- No internet required for operation
- Lightweight and fast
- Reliable data storage
- File-based database (pharmacy.db)

**4. Node.js**
- Server environment
- Handles API requests
- Processes data
- Required to run the system

### Supporting Libraries

**UI Components:**
- **Tailwind CSS**: Modern, professional styling
- **Lucide Icons**: Clear, consistent icons
- **SweetAlert2**: Beautiful alert messages

**Data Handling:**
- **XLSX**: Excel file generation
- **jsPDF**: PDF document creation
- **Papa Parse**: CSV file processing

**Authentication:**
- **bcrypt**: Secure password hashing
- **Cookies**: Session management

**Database:**
- **better-sqlite3**: Fast database operations
- **SQLite3**: Data storage engine

---

## Installation Requirements

To use PharmaCare on your computer, you need to install:

### Step 1: Install Node.js

Node.js is the foundation that runs the system.

**Download and Install:**
1. Go to: https://nodejs.org/
2. Download the LTS (Long Term Support) version
3. Run the installer
4. Follow the installation wizard
5. Restart your computer

**To Verify Installation:**
- Open Command Prompt (Windows) or Terminal (Mac/Linux)
- Type: `node --version`
- You should see a version number (e.g., v18.17.0)
- Type: `npm --version`
- You should see a version number (e.g., 9.6.7)

### Step 2: Install System Dependencies

Once Node.js is installed:

1. Navigate to your PharmaCare folder
2. Open Command Prompt or Terminal in that folder
3. Run this command:
   ```bash
   npm install
   ```
4. Wait for installation to complete (may take a few minutes)

### Step 3: Setup Database

Initialize the database with demo data:

```bash
node setup-database.js
node seed-demo-data.js
```

### Step 4: Start the System

Run this command to start the system:

```bash
npm run dev
```

The system will start and show:
```
Ready on http://localhost:3001
```

### Step 5: Access the System

1. Open your web browser
2. Go to: `http://localhost:3001`
3. You'll see the login page
4. Use the default credentials to login

### System Requirements

**Minimum Requirements:**
- **Operating System**: Windows 10/11, macOS 10.15+, or Linux
- **RAM**: 4 GB (8 GB recommended)
- **Storage**: 500 MB free space
- **Processor**: Intel Core i3 or equivalent
- **Browser**: Chrome, Firefox, Safari, or Edge (latest version)

**Recommended:**
- **RAM**: 8 GB or more
- **Storage**: 2 GB free space
- **Internet**: Not required for operation (only for initial setup)

### Keeping the System Running

**To Start the System:**
```bash
npm run dev
```

**To Stop the System:**
- Press `Ctrl + C` in the Command Prompt/Terminal

**To Restart:**
- Stop the system (Ctrl + C)
- Run `npm run dev` again

### Backup Your Data

Your data is stored in `pharmacy.db` file. To backup:

**Windows:**
```bash
copy pharmacy.db pharmacy.db.backup
```

**Mac/Linux:**
```bash
cp pharmacy.db pharmacy.db.backup
```

Do this regularly to protect your data!

---

## Troubleshooting

### Common Issues and Solutions

**Problem**: Can't login
- **Solution**: Check if server is running (`npm run dev`)
- Verify you're using correct credentials
- Try resetting admin password: `node reset-admin-password.js`

**Problem**: Port 3001 already in use
- **Solution**: Another program is using that port
- Stop other programs or change port in configuration

**Problem**: Database error
- **Solution**: Check if `pharmacy.db` file exists
- Run `node setup-database.js` to recreate

**Problem**: Changes not showing
- **Solution**: Refresh browser page (F5)
- Clear browser cache
- Restart the server

**Problem**: Import fails
- **Solution**: Check CSV format
- Ensure all required columns are present
- Verify data types (numbers for stock and prices)

---

## Best Practices

### Daily Operations

1. **Start of Day:**
   - Login to the system
   - Check dashboard for yesterday's summary
   - Review low stock alerts
   - Check expiring medicines

2. **During Sales:**
   - Always enter customer information when possible
   - Verify medicine selection before completing sale
   - Print or send invoice to customer
   - Check change amount before giving to customer

3. **End of Day:**
   - Review today's sales on dashboard
   - Export daily reports for records
   - Check for any unpaid invoices
   - Backup database if needed

### Inventory Management

1. **Regular Checks:**
   - Weekly inventory count
   - Update stock levels if there are discrepancies
   - Remove expired medicines from system
   - Mark damaged goods appropriately

2. **Reordering:**
   - Set reorder levels for each medicine
   - Monitor low stock alerts daily
   - Use sales trends to predict demand
   - Order before stock runs out

3. **Pricing:**
   - Review prices monthly
   - Update selling prices if costs change
   - Consider profit margins
   - Stay competitive with market prices

### Security

1. **User Accounts:**
   - Give each staff member their own account
   - Never share passwords
   - Use strong passwords (mix of letters, numbers, symbols)
   - Deactivate accounts when staff leaves

2. **Data Protection:**
   - Backup database weekly (minimum)
   - Keep backups in safe location
   - Limit admin access to trusted staff
   - Review activity logs periodically

3. **System Access:**
   - Don't leave system unattended while logged in
   - Always logout at end of shift
   - Lock computer if stepping away
   - Close browser when done

---

## Support and Help

### Getting Help

If you encounter issues or need assistance:

1. **Check This Manual**: Most answers are here
2. **Review Error Messages**: They often tell you what's wrong
3. **Check Activity Logs**: See what actions were taken
4. **Verify Database**: Run `node verify-system.js`

### System Maintenance

**Regular Tasks:**
- Daily: Backup database
- Weekly: Review activity logs
- Monthly: Clear old activity logs if needed
- Quarterly: Review and update user accounts

### System Updates

To update the system when new versions are available:

```bash
# Stop the current system (Ctrl + C)
# Pull new updates
npm install
# Restart
npm run dev
```

---

## Conclusion

PharmaCare Management System is designed to make your pharmacy operations smooth and efficient. With proper use, it will help you:

- Save time on daily operations
- Reduce errors in sales and inventory
- Make better business decisions with reports
- Track medicine sales and profit accurately
- Manage staff access and responsibilities
- Keep accurate records for accounting

**Remember:**
- Take time to explore all features
- Use reports to understand your business
- Keep your data backed up regularly
- Train all staff on proper system use

For the best experience, ensure all staff understand their role's capabilities and follow the best practices outlined in this manual.

---

**System Version**: 1.0 (Complete)  
**Last Updated**: December 2024  
**Status**: Production Ready

*This manual covers all features of the PharmaCare Management System. For technical support or customization, contact your system administrator.*
