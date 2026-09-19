# 🚦 Indore Route Pathfinder

<div align="center">

![React](https://img.shields.io/badge/React-20232A?style=for-the-badge\&logo=react\&logoColor=61DAFB)

![Node.js](https://img.shields.io/badge/Node.js-43853D?style=for-the-badge\&logo=node.js\&logoColor=white)

![MongoDB](https://img.shields.io/badge/MongoDB-4EA94B?style=for-the-badge\&logo=mongodb\&logoColor=white)

**A simple web application to plan routes between stations in Indore using Dijkstra's Algorithm**

</div>

---

## ✨ What it does

* 📍 **Add Stations**: Create new stations/locations
* 🔗 **Connect Stations**: Link stations with distance and cost
* 🧭 **Find Routes**: Calculate shortest path by distance OR cheapest path by cost
* 📊 **View All**: See all stations and connections in one place

---

## 🛠️ Tech Stack

* **Frontend**: React.js, Tailwind CSS
* **Backend**: Node.js, Express.js
* **Database**: MongoDB
* **Algorithm**: Dijkstra's Shortest Path

---

## 🏃‍♂️ Quick Start

### 1. Clone & Install

```bash
git clone https://github.com/ManiChandana1215/PathFinder.git

cd PathFinder

# Backend
cd backend && npm install

# Frontend
cd ../frontend && npm install
```

### 2. Setup Environment

Create `.env` in the backend folder:

```env
MONGO_URI=your_mongodb_connection_string
PORT=5000
```

### 3. Run Application

```bash
# Start backend (Terminal 1)
cd backend && npm run dev

# Start frontend (Terminal 2)
cd frontend && npm run dev
```

Open the frontend URL shown by Vite in your browser.

---

## 🎯 How to Use

1. **Add Stations**: Enter a station name and click "Add Station".
2. **Connect Stations**: Select two stations, enter distance (km) and cost (₹), then click "Add Connection".
3. **Find Route**: Choose start/end stations and select "Distance" or "Cost" optimization.
4. **View Results**: See the optimal path with total distance and cost.

---

## 📁 Project Structure

```text
PathFinder/

├── frontend/          # React application
│   ├── src/
│   │   └── App.jsx    # Main component
│   └── package.json
│
├── backend/           # Express API
│   ├── models/        # MongoDB schemas
│   ├── routes/        # API routes
│   ├── utils/         # Dijkstra algorithm
│   └── server.js      # Main server
│
└── README.md
```

---

## 🔌 API Endpoints

```text
GET    /api/stations       # Get all stations
POST   /api/stations       # Add new station

GET    /api/connections    # Get all connections
POST   /api/connections    # Add new connection

POST   /api/route          # Calculate optimal route
```

---

## 🧮 Algorithm

The application uses **Dijkstra's Algorithm** to find optimal routes.

* **Shortest Distance**: Finds the route with minimum total distance in kilometers.
* **Cheapest Cost**: Finds the route with minimum total cost in rupees.

The algorithm treats stations as **nodes** and connections between stations as **edges**, with distance or cost used as the edge weight.

---

## 🤝 Contributing

1. Fork the repository.
2. Create a feature branch:

```bash
git checkout -b feature-name
```

3. Commit your changes:

```bash
git commit -m "Add feature"
```

4. Push the branch:

```bash
git push origin feature-name
```

5. Open a Pull Request.

---

## 📬 Contact

**Made by Mani Chandana**

* 📧 Email: [manichandana1512@gmail.com](mailto:manichandana1512@gmail.com)
* 💻 GitHub: [ManiChandana1215](https://github.com/ManiChandana1215)

---
