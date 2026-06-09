# Route Planner

A full-stack Route Planner application that allows users to create locations, connect routes between locations, and find optimal paths using graph algorithms.

## Features

* Add and manage locations/stations
* Create connections between locations
* Visualize routes using an interactive graph
* Find shortest routes using Dijkstra's Algorithm
* Find routes using Breadth First Search (BFS)
* Route cost and distance calculation
* Interactive route highlighting
* Responsive user interface

## Tech Stack

### Frontend

* React
* Axios
* React Flow / XYFlow
* CSS

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose

## Project Structure

```bash
RoutePlanner/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── models/
│   ├── routes/
│   ├── controllers/
│   ├── server.js
│   └── package.json
│
└── README.md
```

## Installation

### Clone the Repository

```bash
git clone <repository-url>
cd RoutePlanner
```

### Backend Setup

```bash
cd backend
npm install
```

Create a `.env` file inside the backend folder:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
```

Start the backend server:

```bash
npm start
```

or

```bash
nodemon server.js
```

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

The frontend will run on:

```bash
http://localhost:5173
```

## API Endpoints

### Stations

| Method | Endpoint          | Description      |
| ------ | ----------------- | ---------------- |
| GET    | /api/stations     | Get all stations |
| POST   | /api/stations     | Create a station |
| PUT    | /api/stations/:id | Update a station |
| DELETE | /api/stations/:id | Delete a station |

### Routes

| Method | Endpoint    | Description         |
| ------ | ----------- | ------------------- |
| POST   | /api/routes | Create a connection |
| GET    | /api/routes | Get all connections |

## Algorithms Used

### Dijkstra's Algorithm

Used to find the shortest weighted path between locations.

### Breadth First Search (BFS)

Used to find paths based on minimum number of stops.

## Future Enhancements

* User authentication
* Route history
* Real-time traffic integration
* Interactive maps
* Route optimization suggestions

## Author

Vishakha Gautam
