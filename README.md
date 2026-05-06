# ⚽ TurfSync – Turf Schedule Management System

![TurfSync Banner](https://5.imimg.com/data5/SELLER/Default/2025/1/478645771/CA/NP/GI/25194007/turfsync-turf-booking-management-system-software.jpg)

> **Course:** CSC 2210: Object Oriented Programming 2 (Fall 2025-2026)  
> **Institution:** American International University–Bangladesh (AIUB)

**TurfSync** is a desktop-based application developed using **C# Graphical User Interface (GUI)** with SQL Server database integration. It is designed to digitize and automate the manual process of turf scheduling, booking, maintenance, and service evaluation.

---

## 📌 Project Overview

Traditional turf management relies on phone calls and handwritten registers, leading to double bookings and poor tracking. **TurfSync** solves this by simulating a real-life management environment using **Object-Oriented Programming (OOP)** concepts such as encapsulation, modularity, and role-based access control.

**Key Highlights:**
* **Role-Based Access:** Secure login for Admin, Manager, Staff, and Players.
* **Real-Time Scheduling:** Dynamic status updates (Available, Booked, Maintenance).
* **Database Normalization:** Database structured up to **2NF** to ensure data integrity.
* **Feedback System:** Players can rate service quality, lighting, and turf condition.

---

## 👥 User Roles & Features

### 1️⃣ Admin (System Administrator)
* **User Management:** Add/Edit/Manage Staff and Managers with assigned roles.
* **Location Management:** Configure multiple turf locations, operating hours, and rules.
* **Package Configuration:** Create turf packages and pricing slots.
* **Manual Booking:** Record bookings on behalf of walk-in customers.

### 2️⃣ Turf Manager
* **Dashboard:** View revenue, total bookings, and pending requests.
* **Schedule Control:** Update slot status (Available/Maintenance) and approve/reject booking requests.
* **Dynamic Pricing:**
    * *Night Pricing:* Auto-charge for slots after 6 PM.
    * *Weekend Pricing:* Auto-charge for Fridays/Saturdays.
* **Maintenance Mode:** Mark specific slots as "Under Maintenance" to prevent bookings.

### 3️⃣ Player (Customer)
* **Booking System:** Search slots by date/location and book available times.
* **Cancellation Rules:**
    * Cannot cancel if less than **2 hours** remain before the match.
    * **80% Refund** calculated automatically for valid cancellations.
* **Rescheduling:** Move bookings to new slots (allowed if >2 hours remain).
* **Rating & History:** View played matches and rate specific aspects (Light, Equipment, Cleanliness).

### 4️⃣ Staff (On-Ground Operations)
* **Ground Preparation:** Track tasks like "Turf Brushed," "Trash Cleaned," and "Bottles Removed."
* **Facility Status:** Update status for Lights (On/Off), Bibs, Cones, and Footballs.
* **Attendance Tracking:** Confirm player arrival (Required for players to leave ratings later).

---

## 🛠️ Tech Stack

* **Language:** C#
* **Framework:** .NET Desktop Application (GUI)
* **Database:** SQL Server
* **Design Pattern:** Layered Architecture with OOP Principles
* **Database Design:** Normalized to Second Normal Form (2NF)

---

## 🗂️ Database Schema

The system utilizes a structured relational database with the following key entities:
* **Users:** Stores Admin, Manager, Staff, and Player credentials.
* **TurfSchedule:** Manages slots, prices, and status.
* **PendingRequest & BookingHistory:** Tracks active, completed, and cancelled bookings.
* **StaffManagement:** Logs maintenance tasks and equipment status.
* **ServiceRating:** Stores detailed user feedback.

---

## 🚀 Installation & Setup

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/fairuzfaiyaz/TurfSyncTurfSchedulingSportsSystem.git](https://github.com/fairuzfaiyaz/TurfSyncTurfSchedulingSportsSystem.git)
    ```
2.  **Database Setup:**
    * Open **SQL Server Management Studio (SSMS)**.
    * Run the provided `TurfSyncDB.sql` script to generate tables and relationships.
    * Update the **Connection String** in the C# project configuration.
3.  **Run Application:**
    * Open the solution file (`.sln`) in **Visual Studio**.
    * Build and Run the project.

---

### TEAM KINGSMAN  
**Group:** 6  **Section:** U  

| SL | Student Name | Student ID |
| :-- | :-- | :-- |
| 1 | Fairuz Faiyaz | 23-54707-3 |
| 2 | Md. Iftakher Hossain | 23-54694-3 |
| 3 | Tariqul Islam | 23-54685-3 |
| 4 | Tahosin Iftiak Tonoy | 23-54682-3 |
| 5 | Md. Ariful Hoque | 23-54680-3 |

**Supervised By:** Md. Sazid Uddin

---

_This project was submitted as part of the SWE[U] course requirements._
