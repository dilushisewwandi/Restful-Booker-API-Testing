# 🧪 Restful Booker API Testing (Postman Project)

This is a complete Postman collection designed to test the **Restful Booker API**. It covers **authentication**, **booking creation**, and all **CRUD operations** using real-world testing practices. This project demonstrates how to automate API testing flows and manage dynamic data with Postman environments and scripts.

---

## ✅ Features Covered

- 🔐 **Token-based authentication** (using `/auth`)
- 📝 **Create Booking** (with test script to save booking ID)
- 🔍 **Get All Bookings** and **Get by ID**
- ♻️ **Update Booking** (PUT)
- 🧩 **Partial Update Booking** (PATCH)
- 🗑️ **Delete Booking**
- 💡 **Health Check** (`/ping` endpoint)

---

## 📂 Collection Highlights

- Uses **Postman environment variables** (`base_url`, `token`, `bookingId`)
- Applies **Postman test scripts** to:
  - Save token after auth
  - Save `bookingId` after creating a booking
- Sends authenticated requests using `Cookie: token={{token}}`
- Demonstrates **request chaining**, status validation, and dynamic workflows

---

## 🔧 How to Use

1. **Import the Collection**
   - Download or clone this repo
   - Open Postman → Import → Upload `Restful Booker API.postman_collection.json`

2. **Create an Environment**
   - Variable: `base_url`
   - Value: `https://restful-booker.herokuapp.com`
   - Run the **Auth** request to store `{{token}}`
   - Run the **Create Booking** request to store `{{bookingId}}`

3. **Run Each Request**
   - Try `GET`, `PUT`, `PATCH`, and `DELETE` on the booking you created

---

## 📚 Learning Goals

- Practice **real-world API testing**
- Understand **token authentication**
- Automate test flows using **Postman scripts**
- Use **Postman variables** to reuse and chain requests
