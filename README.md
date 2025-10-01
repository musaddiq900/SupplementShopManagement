# Supplement Shop Management System

## Project Overview

A comprehensive desktop application designed to streamline supplement shop operations with robust inventory management, sales processing, and administrative controls. Built with Python Tkinter for the frontend and MySQL for reliable data storage.

## 🚀 Key Features

### 👨‍💼 Admin Module
- **Employee Management**: Add, edit, and manage staff accounts with role-based permissions
- **Supplier Management**: Maintain supplier database with contact and product information
- **Product Catalog**: Comprehensive product management with categories and pricing
- **Inventory Tracking**: Real-time stock level monitoring and low stock alerts
- **Sales Analytics**: Dashboard with sales reports and performance metrics
- **Category Management**: Organize products into logical categories

### 💼 Employee Module
- **Point of Sale (POS)**: Fast and efficient billing system
- **Customer Management**: Process purchases and maintain customer records
- **Inventory Lookup**: Quick product search and availability checking
- **Sales Processing**: Generate invoices and process payments

### 📊 Core System Features
- **Real-time Inventory**: Automatic stock updates with purchase transactions
- **Billing System**: Generate detailed invoices with tax calculations
- **Sales Reporting**: Comprehensive sales data and analytics
- **User Authentication**: Secure login with role-based access control
- **Data Backup**: Automated database backup and recovery

## 🛠 Technology Stack

### Frontend
- **Python 3.8+**
- **Tkinter** - Native GUI framework
- **CustomTkinter** - Enhanced UI components
- **Pillow (PIL)** - Image processing for product photos

### Backend & Database
- **MySQL 8.0** - Relational database management
- **MySQL Connector/Python** - Database connectivity
- **SQLAlchemy** - ORM for database operations

### Additional Libraries
- **NumPy** - Data analysis and calculations
- **Matplotlib** - Sales charts and reporting
- **ReportLab** - PDF invoice generation
- **DateTime** - Transaction timestamping

## 📁 Project Structure

```
supplement_shop_management/
│
├── src/
│   ├── main.py                 # Application entry point
│   ├── database/
│   │   ├── __init__.py
│   │   ├── connection.py       # Database connection handler
│   │   ├── models.py          # Database schema and models
│   │   └── queries.py         # SQL queries and procedures
│   │
│   ├── modules/
│   │   ├── __init__.py
│   │   ├── admin.py           # Admin dashboard and management
│   │   ├── employee.py        # Employee billing interface
│   │   ├── inventory.py       # Product and stock management
│   │   ├── sales.py           # Sales processing and reporting
│   │   └── auth.py            # User authentication system
│   │
│   ├── ui/
│   │   ├── __init__.py
│   │   ├── components/        # Reusable UI components
│   │   ├── themes/            # Application styling
│   │   └── windows/           # Main application windows
│   │
│   └── utils/
│       ├── __init__.py
│       ├── validators.py      # Input validation utilities
│       ├── helpers.py         # Common helper functions
│       └── constants.py       # Application constants
│
├── data/
│   ├── database/
│   │   └── shop_management.sql    # Database schema
│   ├── images/                # Application images and icons
│   └── reports/               # Generated reports and invoices
│
├── docs/                      # Project documentation
├── tests/                     # Unit and integration tests
├── requirements.txt           # Python dependencies
└── README.md                  # Project documentation
```

## 🗄 Database Schema

### Core Tables
- **users** - User accounts and authentication
- **employees** - Employee details and roles
- **suppliers** - Supplier information
- **categories** - Product categorization
- **products** - Product catalog with pricing
- **inventory** - Stock levels and tracking
- **customers** - Customer information
- **sales** - Sales transaction records
- **sale_items** - Individual sale line items
- **purchases** - Supplier purchase orders

## 🚀 Installation & Setup

### Prerequisites
- Python 3.8 or higher
- MySQL Server 8.0
- Git

### Step 1: Clone Repository
```bash
git clone https://github.com/musaddiq900/SupplementShopManagement.git
cd supplement-shop-management
```

### Step 2: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 3: Database Configuration
1. Create MySQL database:
```sql
CREATE DATABASE supplement_shop;
```

2. Import database schema:
```bash
mysql -u username -p supplement_shop < data/database/shop_management.sql
```

### Step 4: Configure Application
Create `config.ini` file:
```ini
[database]
host = localhost
user = your_username
password = your_password
database = supplement_shop

[application]
name = Supplement Shop Management
version = 1.0.0
theme = dark-blue
```

### Step 5: Run Application
```bash
python src/main.py
```

## 💡 Usage Guide

### For Administrators
1. **Login** with admin credentials
2. **Manage Employees** - Add staff and assign roles
3. **Update Inventory** - Add new products and categories
4. **View Reports** - Analyze sales and performance metrics
5. **Supplier Management** - Maintain supplier relationships

### For Employees
1. **Login** with employee credentials
2. **Access Billing Module** - Process customer purchases
3. **Search Products** - Quick product lookup
4. **Generate Invoices** - Create professional bills
5. **Update Stock** - Process inventory changes

## 🔧 Configuration Options

### Database Settings
- Connection pooling
- Query timeout settings
- Backup automation
- Performance optimization

### Application Settings
- UI themes and styling
- Receipt template customization
- Tax calculation rules
- Discount policies

## 📈 Reporting Features

- **Daily Sales Reports**
- **Inventory Status Reports**
- **Employee Performance Metrics**
- **Supplier Purchase History**
- **Customer Purchase Patterns**

## 🔒 Security Features

- **Password encryption**
- **Role-based access control**
- **Session management**
- **Audit trails**
- **Data validation**

## 🤝 Contributing

1. Fork the repository
2. Create feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit changes (`git commit -m 'Add AmazingFeature'`)
4. Push to branch (`git push origin feature/AmazingFeature`)
5. Open Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

For support and queries:
- Create an issue in the GitHub repository
- Email: musaddiqa00@gmail.com


## 🗺 Future Enhancements

- [ ] Mobile companion app
- [ ] Online ordering integration
- [ ] Barcode scanning support
- [ ] Multi-language support
- [ ] Cloud backup integration
- [ ] Advanced analytics dashboard
- [ ] CRM integration
- [ ] Email marketing module

---

**Developed with ❤️ for supplement shop businesses**
