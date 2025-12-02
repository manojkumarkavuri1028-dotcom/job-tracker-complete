# 🚀 COMPLETE DEPLOYMENT GUIDE

## ⚡ Quick Deploy (EASIEST METHOD)

### All code files are available in Google Docs:
**📄 Complete Code Package:** https://docs.google.com/document/d/1fhFKgdPUmQ-JW7gwjSLY8OixurqtGeciHbuupm9PB8Y/edit

---

## 📥 **Method 1: WinSCP Download (RECOMMENDED)**

1. **Open WinSCP** and connect to your server:
   - Host: `51.20.98.110`
   - Port: `22`
   - Username: `ubuntu`
   - Private Key: `backend-server-key.pem`

2. **Navigate to** `/backend-app/`

3. **Open the Google Docs link above** and copy each file:
   - Create folder structure as shown in the doc
   - Copy-paste each file content from Google Docs
   - Save files in correct locations

---

## 🔧 **Method 2: SSH Direct Commands**

SSH into your server and run:

```bash
cd /backend-app

# Install dependencies
npm install

# Restart server
pm2 stop all
pm2 start server.js --name job-tracker

# Check status
pm2 status

# View logs
pm2 logs job-tracker
```

---

## 📦 **Files You Need (13 Total)**

### Backend Files:
1. ✅ `package.json` (ALREADY IN GITHUB)
2. `server.js`
3. `src/config/database.js`
4. `src/controllers/authController.js`
5. `src/controllers/jobController.js`
6. `src/controllers/companyController.js`
7. `src/routes/authRoutes.js`
8. `src/routes/jobRoutes.js`
9. `src/routes/companyRoutes.js`
10. `src/middleware/auth.js`

### Frontend Files:
11. `public/dashboard.html`
12. `public/styles.css`
13. `public/script.js`

**ALL FILES ARE IN THE GOOGLE DOCS LINK ABOVE** ⬆️

---

## ✅ After Deployment

1. Visit: http://51.20.98.110:3000
2. Register a new account
3. Start tracking your jobs!

---

## 🆘 **Need Help?**

**If the Google Docs link doesn't work:**
- The repository will be updated with all files soon
- Check the README.md for alternative download methods

**Having deployment issues?**
- Make sure port 3000 is open in AWS security groups
- Check pm2 logs: `pm2 logs job-tracker`
- Verify npm dependencies installed: `npm list`
