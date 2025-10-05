🚀 Overview      ------  Created by Sagarika...........

This project is a Single Page Web Application (SPA) developed using React.js and .NET Core Web API that integrates Google APIs for authentication and data access.
It demonstrates enterprise-level design — with secure OAuth 2.0 login, RESTful communication, and clean separation between frontend and backend layers.

🧠 Key Features

🔐 Google OAuth 2.0 Authentication — secure user login using Google credentials.

🗂 Google Drive API Integration — list, view, and download user files.

⚡ Single Page Architecture — React Router–based dynamic navigation without reloads.

🧱 .NET Core Web API Backend — provides authentication validation, token handling, and API services.

🧩 Clean Architecture — Controller → Service → Repository → Database layering for maintainability.

🎨 Modern Responsive UI — built using Tailwind CSS / Material UI.

🧰 Tech Stack

Frontend: React.js, Axios, React Router, Tailwind CSS
Backend: .NET 6 / .NET 8 Web API, Entity Framework Core
Database: SQL Server
Authentication: Google OAuth 2.0
API Integration: Google Drive API
Deployment (optional): Azure App Service / Vercel

⚙️ Setup & Installation
1️⃣ Clone Repository
git clone https://github.com/yourusername/google-spa-webapp.git
cd google-spa-webapp

2️⃣ Configure Google Cloud Credentials

Visit Google Cloud Console
.

Create a new project → Enable Google Drive API.

Generate OAuth 2.0 Client ID & Secret.

Add authorized redirect URIs:

http://localhost:3000 (Frontend)

https://localhost:5001/signin-google (Backend)

3️⃣ Backend Setup (.NET Core API)

Go to /backend folder.

Update appsettings.json with Google Client ID, Secret, and DB connection string.

Example:

"GoogleAuthSettings": {
  "ClientId": "YOUR_GOOGLE_CLIENT_ID",
  "ClientSecret": "YOUR_GOOGLE_CLIENT_SECRET",
  "RedirectUri": "https://localhost:5001/signin-google"
},
"ConnectionStrings": {
  "DefaultConnection": "Server=.;Database=GoogleSPA_DB;Trusted_Connection=True;"
}


Then run:

cd backend
dotnet restore
dotnet run

4️⃣ Frontend Setup (React SPA)
cd frontend
npm install
npm start

5️⃣ Access Application

👉 Open: http://localhost:3000

📂 Project Structure
/google-spa-webapp
│
├── /frontend/               # React.js SPA
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── App.js
│   └── package.json
│
├── /backend/                # .NET Core Web API
│   ├── Controllers/
│   ├── Services/
│   ├── Repository/
│   ├── Models/
│   └── appsettings.json
│
└── README.md











│
└── README.md
