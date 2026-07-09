# 🏥 Hospital Management System

A full-stack Hospital Management System built using **React**, **Node.js**, **Express**, and **MongoDB Atlas**. The application allows users to admit, update, search, discharge, and delete patient records through a clean and responsive interface.

---

## 🚀 Features

* Add (Admit) a new patient
* View all patient records
* Update patient details
* Discharge patients
* Delete patient records
* Search patients by name or disease
* Filter patients by status (Admitted/Discharged)
* Pagination
* Dark Mode / Light Mode
* MongoDB Atlas database
* REST API using Express and Mongoose

---

## 🛠 Technologies Used

### Frontend

* React
* Vite
* CSS
* Fetch API

### Backend

* Node.js
* Express.js
* Mongoose
* CORS

### Database

* MongoDB Atlas

---

## 📁 Project Structure

```text
Hospital-Management/
│
├── backend/
│   ├── index.js
│   ├── package.json
│   └── node_modules/
│
└── frontend/
    ├── src/
    │   ├── App.jsx
    │   ├── App.css
    │   └── main.jsx
    ├── package.json
    └── vite.config.js
```

---

## 📦 Install Backend

Navigate to the backend folder:

```bash
cd backend
```

Install dependencies:

```bash
npm install express cors mongoose
```

Run the backend server:

```bash
node index.js
```

Server starts at:

```text
http://localhost:5000
```

---

## 💻 Install Frontend

Navigate to the frontend folder:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the React application:

```bash
npm run dev
```

Frontend runs at:

```text
http://localhost:5173
```

---

## 🌐 MongoDB Atlas Configuration

Update the connection string in `backend/index.js`:

```javascript
const MONGODB_URI =
"mongodb+srv://<username>:<password>@cluster.mongodb.net/hospitalDB?retryWrites=true&w=majority";
```

Replace:

* `<username>` with your MongoDB username
* `<password>` with your MongoDB password

---

## 📡 REST API Endpoints

### Create Patient

```
POST /patients
```

### Get All Patients

```
GET /patients
```

Supports:

```
?page=1
&limit=5
&search=fever
&status=Admitted
```

### Get Single Patient

```
GET /patients/:id
```

### Update Patient

```
PUT /patients/:id
```

### Delete Patient

```
DELETE /patients/:id
```

---

## 📄 Patient Schema

```javascript
{
  name: String,
  age: Number,
  gender: String,
  disease: String,
  doctorAssigned: String,
  roomNumber: String,
  status: "Admitted" | "Discharged",
  admissionDate: Date,
  dischargeDate: Date
}
```

---

## ▶️ How to Run the Project

### Terminal 1

```bash
cd backend
node index.js
```

### Terminal 2

```bash
cd frontend
npm run dev
```

Open your browser:

```
http://localhost:5173
```

---

## 📷 Application Features

* 🏥 Admit Patient
* ✏️ Edit Patient Record
* 🔍 Search Patients
* 📄 Pagination
* 🚪 Discharge Patient
* 🗑 Delete Patient
* 🌙 Dark Mode
* 📅 Admission & Discharge Dates
* 📱 Responsive Design

---

## 👨‍💻 Author

**Soujanya Baligar**

---

## 📜 License

This project is developed for learning and educational purposes.
