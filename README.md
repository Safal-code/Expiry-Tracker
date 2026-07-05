# 🛒 Expiry Tracker

A full-stack web application that helps users track the expiry dates of medicines, groceries, cosmetics, documents, and other items. The application automatically sends browser push notifications before an item expires using **Firebase Cloud Messaging (FCM)**, helping users avoid waste and stay organized.

---

## 🚀 Features

- User authentication
- Add, edit, and delete expiry items
- Categorize items
- Custom reminder settings (e.g., 7 days, 3 days, 1 day before expiry)
- Browser push notifications using Firebase Cloud Messaging (FCM)
- Automatic reminder scheduling
- Responsive user interface
- Secure backend APIs

---

## 🛠️ Tech Stack

### Frontend
- React.js
- HTML5
- CSS3
- JavaScript

### Backend
- Node.js
- Express.js

### Database
- MongoDB
- Mongoose

## 💡 How Push Notifications Work

- The browser requests notification permission.
- Firebase generates an FCM token.
- The token is stored in MongoDB through the backend.
- A scheduled cron job checks for items whose reminder date matches the current date.
- The backend sends a notification request to Firebase using the stored FCM token.
- Firebase delivers the notification to the registered browser or device.

---

## 📌 Future Improvements
- Notification history
- Analytics dashboard
  

### Notifications
- Firebase Cloud Messaging (FCM)
- Firebase Admin SDK
