# Book Management System (BMS)

A full-stack web application for managing book distribution across colleges and departments. Built using React.js (frontend), Node.js + Express (backend), and MongoDB (database).

---

## 🌟 Features

### 👨‍🎓 Student Side (accessed by Admin and SuperAdmin)
- Login and view issued books
- View remaining books to be issued
- Clean and modern UI

### 🛠️ Admin/SuperAdmin Side
- Add, view, and manage student records
- Filter students by college, department, year, and class
- Bulk upload student details from Excel
- Assign books manually or from inventory
- Track issued and remaining books
- Prevent duplicate book assignments
- Manage book inventory and vendors
- Role-based dashboards (Admin vs SuperAdmin)

---

## 🧰 Tech Stack

| Frontend    | Backend       | Database | Others         |
|-------------|---------------|----------|----------------|
| React.js    | Node.js       | MongoDB  | Express, Mongoose |
| TailwindCSS | Express.js    | Compass  | SweetAlert2, Axios |

---

## 📂 Project Structure (Overview)
BMS-app/<br>
│<br>
├── server/ # Node.js & Express backend<br>
│ ├── routes/<br>
         |──admin.js<br>
         |──auth.js<br>
         |──bookInventoryRoutes.js<br>
         |──student.js<br>
         |──vendorRoutes.js<br>
│ ├── seedFakeStudent.js<br>
│ ├── seedVendorInventory.js<br>
│ ├── server.js<br>
│ |──package-lock.json<br>
│ |──package.json<br>
|
|
├── client/ <br>                        # React frontend
│   ├── public/<br>
│   ├── node_modules/<br>
│   └── src/<br>
│       ├── components/<br>
│       │   ├── AddAdmin.js<br>
│       │   ├── AddBooksPage.js<br>
│       │   ├── AddStudentPage.js<br>
│       │   ├── AdminDashboard.js<br>
│       │   ├── AdminLayout.js<br>
│       │   ├── Login.js<br>
│       │   ├── Logout.js<br>
│       │   ├── Navbar.css<br>
│       │   ├── StudentDetails.js<br>
│       │   ├── StudentDetails.css<br>
│       │   ├── StudentManagementPage.js<br>
│       │   ├── StudentManagement.css<br>
│       │   ├── SuperAdminDashboard.js<br>
│       │   ├── SuperAdminDashboard.css<br>
│       │   ├── SuperAdminLayout.js<br>
│       │   ├── VendorDetails.js<br>
│       │   ├── VendorManagement.js<br>
│       │   ├── VendorManagement.css<br>
│       ├── config/<br>
│       ├── App.js<br>
│
└── README.md



---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/yourusername/BMS-app.git
cd BMS-app
```

### 2. Setup Backend

cd server //backend
npm install
# Create .env file
touch .env
# Add your MongoDB URI inside .env
# MONGO_URI=mongodb://localhost:27017/Student_database
npm start

### Setup Frontend

cd client //frontend
npm install
npm start

The app should now be running at http://localhost:3000

 ### 3.Environment Variables
 Create a .env file in backend/ with the following variables:
 MONGO_URI=your_mongodb_uri
PORT=5000




