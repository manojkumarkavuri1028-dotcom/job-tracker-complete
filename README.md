# 🚀 Job Tracker - Complete Platform

Professional job tracking platform inspired by Teal HQ - Complete Node.js/Express backend with SQLite database and modern UI.

## 📦 Quick Download & Deploy

### Method 1: Direct Download to Server (EASIEST)

SSH into your server and run:

```bash
cd /backend-app
curl -L https://docs.google.com/document/d/1fhFKgdPUmQ-JW7gwjSLY8OixurqtGeciHbuupm9PB8Y/export?format=txt > deployment-guide.txt
```

Or use WinSCP to download from this Google Doc:
**https://docs.google.com/document/d/1fhFKgdPUmQ-JW7gwjSLY8OixurqtGeciHbuupm9PB8Y/edit**

### Method 2: Clone this Repository

```bash
git clone https://github.com/manojkumarkavuri1028-dotcom/job-tracker-complete.git
cd job-tracker-complete
npm install
```

## ✨ Features

- ✅ User Authentication (Login/Register)
- ✅ Job Board with Status Tracking
- ✅ Dashboard with Statistics
- ✅ Company Management
- ✅ Teal HQ-inspired Professional UI
- ✅ SQLite Database
- ✅ RESTful API
- ✅ JWT Authentication

## 🎯 Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: SQLite3
- **Auth**: JWT, bcryptjs
- **Frontend**: HTML5, CSS3, JavaScript
- **Style**: Teal-inspired modern design

## 🚀 Deployment Instructions

### Requirements
- Node.js 14+
- npm or yarn
- Port 3000 available

### Setup Steps

1. **Install Dependencies**
```bash
npm install
```

2. **Start Server**
```bash
node server.js
# OR
pm2 start server.js --name job-tracker
```

3. **Access Application**
```
http://your-server-ip:3000
```

## 📁 Project Structure

```
/backend-app/
├── server.js
├── package.json
├── src/
│   ├── config/
│   │   └── database.js
│   ├── controllers/
│   │   ├── authController.js
│   │   ├── jobController.js
│   │   └── companyController.js
│   ├── routes/
│   │   ├── authRoutes.js
│   │   ├── jobRoutes.js
│   │   └── companyRoutes.js
│   └── middleware/
│       └── auth.js
└── public/
    ├── index.html
    ├── login.html
    ├── dashboard.html
    ├── jobs.html
    ├── companies.html
    ├── styles.css
    └── script.js
```

## 🔗 API Endpoints

### Auth
- `POST /api/auth/register` - Register new user
- `POST /api/auth/login` - Login user

### Jobs
- `GET /api/jobs` - Get all jobs
- `POST /api/jobs` - Create job
- `GET /api/jobs/:id` - Get job by ID
- `PUT /api/jobs/:id` - Update job
- `DELETE /api/jobs/:id` - Delete job
- `GET /api/jobs/stats` - Get job statistics

### Companies
- `GET /api/companies` - Get all companies
- `POST /api/companies` - Create company

## 📄 License

MIT License - feel free to use for personal or commercial projects!

## 🙋 Support

For issues or questions, open an issue on GitHub.

---

**Created with ❤️ for job seekers worldwide**
