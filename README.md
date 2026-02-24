✈️ YL Flights – Flight Booking App (MERN Stack)
📌 Introduction

YL Flights is a full-stack Flight Booking Web Application built using the MERN Stack (MongoDB, Express.js, React.js, Node.js).

The platform allows users to:

Search available flights

Book tickets

View and manage bookings

Cancel reservations

It also provides:

Admin dashboard for managing flights and users

Flight operator panel for adding and updating flights

The system is designed to deliver a seamless, secure, and user-friendly flight booking experience.

🏗️ Technical Architecture

The application follows a three-tier architecture:

1️⃣ Frontend (React.js)

User Authentication (Login/Register)

Flight Search

Booking Module

Admin Dashboard UI

2️⃣ Backend (Node.js + Express.js)

REST API Endpoints

Authentication APIs

Flight Management APIs

Booking APIs

Admin APIs

3️⃣ Database (MongoDB)

Collections:

Users

Flights

Bookings

🗂️ ER Diagram Overview

Entities in the system:

User → Can register, login, book flights

Flight → Contains flight details like origin, destination, price, seats

Booking → Stores booking details linked to user

Admin → Manages flights and bookings

Relationships:

One user can have multiple bookings

One flight can have multiple bookings

Admin manages flights and bookings

🚀 Features
👤 User Features

User Registration & Login

Search Flights by:

Departure City

Destination

Date

Book Flights

View Booking History

Cancel Booking

🛠️ Admin Features

Admin Login

Add New Flights

Update Flights

View All Users

View All Bookings

Approve Flight Operators

🧑‍✈️ Flight Operator Features

Operator Login

Add Flights

View Bookings

Manage Routes

🛠️ Prerequisites

Make sure the following are installed:

Node.js

npm

MongoDB (Local or Atlas)

Git

VS Code (or any IDE)

📁 Project Structure
FlightFinderApp/
│
├── client/              # React Frontend
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── context/
│   │   ├── RouteProtectors/
│   │   └── styles/
│   └── package.json
│
├── server/              # Node + Express Backend
│   ├── index.js
│   ├── schemas.js
│   └── package.json
│
└── README.md

Backend Overview
✔️ Express Server

Handles API requests

Uses middleware (CORS, body-parser)

✔️ MongoDB + Mongoose

Schemas:

User Schema

Flight Schema

Booking Schema

✔️ API Routes

/register

/login

/fetch-flights

/fetch-bookings

/add-flight

/update-flight

/cancel-ticket/:id

🔐 Authentication

Password hashing using bcrypt

Login validation

Role-based access (User / Admin / Operator)

Protected routes

📊 Database Schemas
👤 User Schema

username

email (unique)

password

role

✈️ Flight Schema

flightName

flightId

origin

destination

departureTime

arrivalTime

price

totalSeats

🎟️ Booking Schema

userId

flightName

flightId

passengers

coachClass

journeyDate

totalPrice

🔄 Project Milestones
Milestone 1: Setup

Install dependencies

Create folder structure

Milestone 2: Backend

Express server setup

MongoDB connection

CRUD APIs

Milestone 3: Frontend

React setup

UI Design

API Integration

Booking modal

🖼️ UI Modules

Landing Page

Authentication Page

User Bookings Page

Admin Dashboard

Flight Operator Dashboard

Add New Flight Page

