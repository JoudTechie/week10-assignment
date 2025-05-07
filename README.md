# MERN Blog Application

This project is a full-stack blog application built using the MERN stack (MongoDB, Express, React, Node.js).

## 📁 Project Structure




 Deployment Steps

### 1. Clone the Repository

```bash
git clone https://github.com/cw-barry/blog-app-MERN.git
cd blog-app
```

### 2. Install Dependencies

```bash
# Backend
cd backend
npm install

# Frontend
cd ../frontend
pnpm install
```

### 3. Build the Frontend

```bash
pnpm run build
```

### 4. Deploy Frontend to S3

```bash
aws s3 sync dist/ s3://joud-blogapp-frontend
```


---

### 5. Deploy Backend to EC2

1. SSH into your EC2 instance.
2. Start the backend using PM2:

```bash
pm2 start index.js --name "blog-backend"
```

---

## ✅ Deliverables

- ✅ Screenshot of frontend running from S3 URL
- ✅ Screenshot of backend server running via `pm2 list`
- ✅ `curl -I` output showing `200 OK` from S3 URL

---

## 🔗 Live URLs

- **Frontend (S3):** http://joud-blogapp-frontend.s3-website.eu-north-1.amazonaws.com/ 
- **Backend (EC2):** http://13.50.247.78:5000/api/

---

JoudSDA2010