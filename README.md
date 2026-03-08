# MiniLibrary

A comprehensive library management system built with Laravel 12, designed to streamline book borrowing, cataloging, and user management for educational institutions.

## 📚 About MiniLibrary

MiniLibrary is a modern web application that provides efficient library management solutions. The system enables librarians to manage book inventories, track borrowing records, and handle user accounts with ease. Built with Laravel's robust framework and enhanced with Tailwind CSS for a responsive, user-friendly interface.

### Key Features

- **Book Management**: Complete catalog system with author information, ISBN tracking, and categorization
- **User Management**: Separate roles for students and librarians with appropriate permissions
- **Borrowing System**: Streamlined book borrowing and return process with due date tracking
- **Inventory Tracking**: Real-time monitoring of book availability and borrowing history
- **Responsive Design**: Modern, mobile-friendly interface using Tailwind CSS
- **Authentication**: Secure user authentication and authorization system

## 🛠️ Technology Stack

- **Backend**: Laravel 12 (PHP 8.2+)
- **Frontend**: Blade Templates with Tailwind CSS
- **Database**: MySQL/SQLite
- **Authentication**: Laravel Breeze
- **Build Tools**: Vite
- **Testing**: PHPUnit with Pest

## 📋 System Requirements

- PHP 8.2 or higher
- Composer 2.0 or higher
- Node.js 18.0 or higher
- MySQL 8.0 or SQLite 3.0

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd MiniLibrary
   ```

2. **Install dependencies**
   ```bash
   composer install
   npm install
   ```

3. **Environment setup**
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

4. **Database setup**
   ```bash
   php artisan migrate
   php artisan db:seed
   ```

5. **Build assets**
   ```bash
   npm run build
   ```

6. **Start the development server**
   ```bash
   php artisan serve
   ```

## 🏗️ Project Structure

```
MiniLibrary/
├── app/
│   ├── Models/
│   │   ├── User.php          # User authentication
│   │   ├── Student.php       # Student information
│   │   ├── Book.php          # Book catalog
│   │   ├── Author.php        # Author details
│   │   ├── Borrow.php        # Borrowing records
│   │   └── BorrowItem.php    # Individual borrowed items
│   ├── Http/Controllers/     # Application controllers
│   └── Http/Requests/        # Form validation
├── database/
│   ├── migrations/           # Database schema
│   └── seeders/             # Sample data
├── resources/
│   ├── views/               # Blade templates
│   └── js/                  # Frontend JavaScript
└── routes/
    ├── web.php              # Web routes
    └── api.php              # API routes
```

## 👥 Development Team

MiniLibrary was developed by a dedicated team of developers:

### Core Developers
- **Cyrish Mage Cagasan** - Backend Development & Database Design
- **Stephanie Jane Eleccion** - Frontend Development & UI/UX Design
- **Jhib Lourence Rendon** - System Architecture
- **Prixane Jade Gales** - Testing & Quality Assurance
- **Genesis Maraya** - Testing & Quality Assurance

## 📝 Database Schema

The system uses the following main entities:

- **Users**: Authentication and role management
- **Students**: Student information and library accounts
- **Books**: Book catalog with metadata
- **Authors**: Author information and book relationships
- **Borrows**: Borrowing transactions and records
- **Borrow Items**: Individual items within each borrowing transaction

## 🔧 Available Commands

### Development
```bash
# Start development server with hot reload
npm run dev

# Run all services (server, queue, vite)
composer run dev
```

### Testing
```bash
# Run all tests
composer run test

# Run specific test
php artisan test --filter TestName
```

### Database
```bash
# Fresh migration with seeding
php artisan migrate:fresh --seed

# Create new migration
php artisan make:migration create_table_name
```

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

For support and inquiries, please contact the development team or create an issue in the repository.

---

**MiniLibrary** - Simplifying library management, one book at a time. 📖
