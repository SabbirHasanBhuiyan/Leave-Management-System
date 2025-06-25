# Leave Management System

A comprehensive web-based leave management solution designed as part of University of Chittagong ERP system. Built with React.js, Node.js, and MySQL to streamline leave request workflows, administrative coordination, and secure user authentication.

---

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [Architecture](#architecture)
5. [Installation](#installation)
6. [Running the Application](#running-the-application)
7. [Database Schema](#database-schema)
8. [Security Features](#security-features)
8. [Contributing](#contributing)
10. [License](#license)
11. [Contact](#contact)

---

## Introduction
The Leave Management System is a full-stack web application developed as a critical module within the University ERP ecosystem. It provides a seamless, secure platform for:
- **Teachers and Staff** to submit and track leave requests
- **Administrative Staff** to review, approve, and manage leave applications
- **System Administrators** to oversee the entire leave management workflow

Developed as a university-level project, it demonstrates expertise in:
- Modern full-stack web development with React and Node.js
- Secure authentication and authorization systems
- RESTful API design and implementation
- Normalized database schema design
- Responsive UI/UX development

---

## Features
- 🔐 **Secure Authentication**: JWT-based login system with role-based access control
- 📝 **Leave Request Management**: Intuitive form-based leave application submission
- 🔄 **Workflow Coordination**: Multi-level approval process with status tracking
- 📊 **Dashboard Analytics**: Real-time leave statistics and reporting
- 📱 **Responsive Design**: Mobile-friendly interface using modern CSS frameworks
- 📄 **PDF Generation**: Downloadable leave application reports and certificates
- 👥 **Multi-Role Support**: Different interfaces for students, staff, and administrators
- 📈 **Leave Balance Tracking**: Automatic calculation of available leave days
- 🗄️ **Archive Management**: Historical leave data with search and filter capabilities

---

## Tech Stack

### Frontend
- **Framework**: React.js 18.2.0
- **Build Tool**: Vite
- **Styling**: Tailwind CSS, DaisyUI, Flowbite React
- **Icons**: FontAwesome, Lucide React
- **Routing**: React Router DOM
- **HTTP Client**: Axios
- **PDF Generation**: React-PDF, jsPDF, html2canvas
- **State Management**: React Hooks

### Backend
- **Runtime**: Node.js with TypeScript
- **Framework**: Express.js
- **Database**: MySQL 2
- **Query Builder**: Kysely with TypeScript support
- **Authentication**: JWT (JSON Web Tokens)
- **File Upload**: Multer
- **Email Service**: Nodemailer
- **Validation**: Zod
- **Security**: CORS, Cookie Parser
- **Environment**: dotenv

### Development Tools
- **Package Manager**: npm/yarn
- **Development Server**: Nodemon
- **Code Generation**: Kysely Codegen
- **Linting**: ESLint
- **Formatting**: Prettier
- **Type Checking**: TypeScript

---

## Architecture

The system follows a three-tier architecture:
- **Presentation Layer**: React-based responsive UI
- **Business Logic Layer**: Express.js RESTful API with middleware
- **Data Layer**: MySQL with normalized schema design

---

## Installation

### Prerequisites
- Node.js (v16 or higher)
- MySQL Server (v8.0 or higher)
- npm or yarn package manager

### Backend Setup
```bash
# Clone the repository
git clone https://github.com/SabbirHasanBhuiyan/Leave-Management-System.git
cd Leave-Management-System

# Install backend dependencies
cd backend
npm install

# Setup environment variables
cp .env.example .env
# Edit .env with your database credentials and JWT secret

# Setup database
mysql -u root -p < database/schema.sql
mysql -u root -p < database/seed.sql
```

### Frontend Setup
```bash
# Install frontend dependencies
cd ../frontend
npm install

# Setup environment variables
cp .env.example .env
# Edit .env with your API base URL
```

---

## Running the Application

### Development Mode
```bash
# Start backend server (runs on port 5000)
cd backend
npm run dev

# Start frontend development server (runs on port 3000)
cd frontend
npm run dev
```

### Production Build
```bash
# Build frontend for production
cd frontend
npm run build

# Start backend in production mode
cd backend
npm start
```

Access the application at `http://localhost:3000`

---

## Usage

### For Students/Staff
1. **Login**: Use university credentials to access the system
2. **Apply for Leave**: Fill out the leave application form with required details
3. **Track Status**: Monitor application progress through the dashboard
4. **Download Reports**: Generate PDF copies of approved leave certificates

### For Administrators
1. **Review Applications**: Access pending leave requests through admin panel
2. **Approve/Reject**: Make decisions on leave applications with comments
3. **Generate Reports**: Create comprehensive leave statistics and analytics
4. **Manage Users**: Add, edit, or deactivate user accounts

### Key Workflows
- **Leave Application**: Submit → Review → Approval → Email Notification
- **Status Tracking**: Real-time updates on application progress
- **Report Generation**: Automated PDF creation for approved leaves
---

## Security Features
- **JWT Authentication**: Secure token-based authentication
- **Role-Based Access Control**: Different permissions for users and admins
- **Input Validation**: Server-side validation using Zod
- **SQL Injection Prevention**: Parameterized queries with Kysely
- **CORS Protection**: Configured cross-origin resource sharing
- **File Upload Security**: Secure file handling with Multer
- **Password Security**: Encrypted password storage
- **Session Management**: Secure cookie handling

---

## Contributing
We welcome contributions to improve the Leave Management System!

### How to Contribute
1. Fork the repository
2. Create a feature branch: `git checkout -b feature/YourFeature`
3. Make your changes and commit: `git commit -m 'Add YourFeature'`
4. Push to the branch: `git push origin feature/YourFeature`
5. Open a Pull Request

### Development Guidelines
- Follow TypeScript best practices
- Maintain consistent code formatting with Prettier
- Write meaningful commit messages
- Add appropriate documentation for new features
- Ensure all tests pass before submitting PR

---

## License
This project is licensed under the **MIT License**.

---

## Contact
**Sabbir Hasan Bhuiyan**  
📧 Email: sabbirhasan675@gmail.com  
💼 LinkedIn: [linkedin.com/in/SabbirHasanBhuiyan](https://linkedin.com/in/SabbirHasanBhuiyan)  
🐙 GitHub: [github.com/SabbirHasanBhuiyan](https://github.com/SabbirHasanBhuiyan)

---

## Acknowledgments
- Developed as part of University ERP System coursework
- Special thanks to 6 ohter team members and the Web Engineering course instructors Dr. Rudra Pratap Deb Nath and Dr. Iqbal Ahmed
- Built with modern web technologies and best practices

---

*This project demonstrates proficiency in full-stack web development, database design, and enterprise application architecture. It showcases the integration of modern frontend and backend technologies to create a production-ready leave management solution.*
