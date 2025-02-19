## **Getting Started**

### 1. **Clone the Repository**
```sh
# Clone the repository
git clone https://github.com/yadavlalita/fb-insight-backend.git
cd fb-insight-backend.git
```

### 2. **Set Up Backend**
```sh
cd backend
npm install
```

#### **Environment Variables (`.env` in backend)**
```
FACEBOOK_APP_ID=your_app_id
FACEBOOK_APP_SECRET=your_app_secret
REDIRECT_URI=http://localhost:5000/auth/facebook/callback
```

#### **Run Backend**
```sh
node server.js
```
## **Deployment**

### **Backend Deployment (Railway/Heroku)**
```sh
# Railway Deployment
git push origin main
# Heroku Deployment
heroku create fb-insights-backend
heroku config:set FACEBOOK_APP_ID=your_app_id
heroku config:set FACEBOOK_APP_SECRET=your_app_secret
heroku config:set REDIRECT_URI=https://fb-insights-backend.herokuapp.com/auth/facebook/callback
git push heroku main
```
