🍔 FoodCompare - Price Comparison App
FoodCompare is a sleek, full-stack web application designed to help users find the best deals on their favorite food items from popular Indian delivery platforms like Zomato, Swiggy, and Uber Eats. By providing a clean interface to search and compare prices, delivery times, and service fees, it ensures you always make the most cost-effective choice.

This project features a responsive React frontend built with Tailwind CSS and a robust Node.js/Express backend that serves simulated, dynamic data.

✨ Key Features
Universal Search: Instantly search for any dish or restaurant across a wide-ranging mock database.

Multi-Platform Comparison: View prices for the same food item from Zomato, Swiggy, and Uber Eats in a clean, comparable table.

Detailed Breakdown: Get insights into not just the item price, but also simulated delivery times and service charges.

Best Deal Highlighting: The cheapest platform for your chosen item is automatically highlighted in green, so you never miss a deal.

Price Difference Calculator: Instantly see how much you can save by choosing the most economical option.

Recent Search History: Quickly re-run your previous searches with a single click, powered by localStorage.

Responsive & Mobile-Friendly: A clean, intuitive UI that works beautifully on all devices, from desktops to smartphones.

Loading & Empty States: A polished user experience with skeleton loaders during data fetching and helpful messages when no results are found.

🚀 Tech Stack
This project is a full-stack application built with modern web technologies.

Frontend:

React.js: A powerful JavaScript library for building user interfaces.

Tailwind CSS: A utility-first CSS framework for rapid, custom UI development.

Headless UI: Unstyled, fully accessible UI components for building the comparison modal.

Backend:

Node.js: A JavaScript runtime for building fast and scalable server-side applications.

Express.js: A minimal and flexible Node.js web application framework for the API.

Database:

Mock data stored in a db.json file, served dynamically by the backend server to simulate a real-world database.

⚙️ How It Works
Since public APIs for food delivery platforms are not available, this application simulates the price comparison process:

The React frontend captures the user's search query.

A request is sent to the /api/search endpoint on the Node.js/Express backend.

The backend filters the db.json file to find matching food items or restaurants.

For each matching item, the server dynamically simulates price variations, delivery times, and service fees for Zomato, Swiggy, and Uber Eats. This ensures that the data feels fresh and different with every search.

The structured JSON response is sent back to the frontend.

The React frontend displays the results as interactive cards. Clicking "Compare Prices" opens a detailed modal with a comparison table and highlights the best deal.

🔧 Setup and Local Installation
To run this project on your local machine, follow these simple steps:

Prerequisites:

Node.js (v14 or higher)

npm (or yarn)

1. Clone the Repository

git clone [https://github.com/your-username/food-comparison-app.git](https://github.com/your-username/food-comparison-app.git)
cd food-comparison-app

2. Set Up the Backend Server

# Navigate to the server directory
cd server

# Install dependencies
npm install

# Start the server (runs on http://localhost:3001)
npm start

3. Set Up the Frontend Client

# Navigate to the client directory from the root folder
cd client

# Install dependencies
npm install

# Start the React development server (runs on http://localhost:3000)
npm start

Once both the server and client are running, open your browser and navigate to http://localhost:3000 to use the application.

📄 API Endpoint
The backend provides one primary API endpoint:

GET /api/search?q=<query>

Fetches all food items from the mock database that match the search <query>.

The query can match either the dish name or the restaurant name.

Returns a JSON array of item objects, each containing the dynamically generated price comparison data across platforms.

💡 Future Improvements
User Authentication: Add user accounts to save favorite items or track order history.

Location-Based Search: Simulate searching for restaurants based on a user's location.

Advanced Filtering: Allow users to filter results by cuisine, price range, or platform.

Real-time Database: Replace the JSON file with a real-time database like Firebase Firestore for more complex interactions.

⚖️ License
This project is licensed under the MIT License. See the LICENSE file for details.
