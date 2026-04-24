# 🏟 Mini Stadium Booking Bot

A fully automated Telegram bot for managing mini stadium reservations.  
Users can book sports fields (Football, Volleyball, Badminton), select time slots, and confirm bookings directly in Telegram.  
Admins can manage all reservations in real-time through a built-in control system.

---

## 📌 Project Overview

The **Mini Stadium Booking Bot** simplifies the stadium reservation process by removing manual communication and replacing it with an automated Telegram-based system.

Users can:
- Check available time slots
- Book a stadium instantly
- Choose game types
- Submit contact details
- Select payment method

Admins can:
- Monitor all bookings
- Confirm or cancel reservations
- Manage daily schedules
- Send announcements

---

## ✨ Features

### 👤 User Features
- 🏟 Stadium information
- 📅 Book available time slots
- ⏰ View free & occupied schedules
- 🎮 Select game type (Football / Volleyball / Badminton)
- 📱 Send phone number (contact or manual input)
- 💳 Choose payment method (Cash / Click / Payme)
- 🗂 View personal booking history
- ⭐ Send feedback

---

### 🛠 Admin Features
- 📋 View daily bookings
- ✅ Confirm reservations
- ❌ Cancel bookings
- 📢 Send announcements to all users
- 📊 Monitor booking activity

---

## ⚙️ Bot Workflow

1. User starts bot (`/start`)
2. Opens "📅 Book Stadium"
3. Selects:
   - Date 📅
   - Time ⏰
   - Game type 🎮
4. Enters phone number 📱
5. Chooses payment method 💳
6. Booking is saved as **pending**
7. Admin reviews and confirms or cancels booking

---

---

## 🗄 Database Schema

### 👤 users
Stores user information and admin roles.

### 📅 bookings
Stores all reservations:
- date
- time
- game type
- payment method
- status (pending / confirmed / canceled)

### ⭐ feedback
Stores user feedback messages.

---

## 🧰 Tech Stack

- Python 3.10+
- Aiogram v3 (Telegram Bot Framework)
- SQLite (aiosqlite)
- FSM (Finite State Machine for booking flow)

---

## 🚀 Installation

```bash
git clone <repo-url>
cd mini_stadion_bot

python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate

pip install -r requirements.txt
