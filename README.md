# ✅ To-Do-List: Advanced Database Design Project

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)

A REST API backend for a hierarchical to-do / checklist system, built for an Advanced Database Design course.

## 🧩 Data model

`Agent` → `Space` → `Category` → `Checklist` → `Item` → `Step`

Each entity has its own Mongoose model, controller and routes, and an **aggregation** route exposes combined queries across collections.

## 🧱 Tech stack

Node.js · Express · MongoDB (Mongoose) · CORS · Morgan · dotenv

## 🗂️ Structure

```
back-end/
├── Server.js     # app entry point
├── Config/       # database connection
├── Models/       # Agents, Space, Category, Checklist, Item, Steps
├── Controller/   # request handlers
└── Routes/       # REST routes + aggregation endpoints
```

## 🚀 Getting started

```bash
git clone https://github.com/Aser-S/To-Do-List.git
cd To-Do-List/back-end
npm install
# create a .env file with your MongoDB connection string
node Server.js
```
