

# 🎥 MovieBookingSystem

**MovieBookingSystem** is a web application that allows users to search, browse, and book movie tickets. Built with ASP.NET for backend functionality and Angular for the frontend, this project demonstrates a full-stack approach to building an interactive, scalable, and user-friendly movie booking system.


## 🎯 Features
- **User Authentication**: Secure login and registration for users.
- **Browse and Search Movies**: Users can search for movies by title, genre, or release date.
- **Seat Selection**: Choose available seats before booking.
- **Booking Confirmation**: Confirmation email for successful bookings.
- **Admin Dashboard**: Admins can manage movie listings, theater schedules, and view bookings.
- **Responsive Design**: Works seamlessly across desktop and mobile devices.

---

## 💻 Tech Stack
### Frontend
- **Angular**: For building a responsive and interactive user interface.
- **HTML5/CSS3/Bootstrap/Angular**: For styling and layout.

### Backend
- **ASP.NET Core**: Web API for managing application logic and handling HTTP requests.
- **Entity Framework Core**: ORM for data access and management.
- **SQL Server**: Database for storing user, movie, and booking data.

### Other Tools
- **JWT Authentication**: Secure user login.
- **Swagger**: API documentation and testing.
- **SendGrid**: For sending booking confirmation emails.

---

## 🚀 Installation

### Prerequisites
- **Node.js**: To run the Angular frontend.
- **ASP.NET Core SDK**: To run the backend server.
- **SQL Server**: For the database.

### Steps
1. **Clone the Repository**
   ```bash
   git clone https://github.com/Bikash432/MovieBookingSystem-ASP.NET.git
   cd MovieBookingSystem
   ```

2. **Backend Setup**
   - Navigate to the `MovieBookingSystem.Api` folder.
   - Update the `appsettings.json` file with your SQL Server connection string and SendGrid API key.
   - Run database migrations to set up the database:
     ```bash
     dotnet ef database update
     ```
   - Start the backend server:
     ```bash
     dotnet run
     ```

3. **Frontend Setup**
   - Navigate to the `MovieBookingSystem.Client` folder.
   - Install Angular dependencies:
     ```bash
     npm install
     ```
   - Start the frontend server:
     ```bash
     ng serve
     ```

---

## 🧑‍💻 Usage
- Access the application at `http://localhost:4200`.
- **User Flow**: Register or log in to the system, browse available movies, choose seats, and complete the booking process.
- **Admin Flow**: Log in as an admin to add new movies, manage schedules, and view bookings.

---

## 📁 Folder Structure
```
MovieBookingSystem/
├── MovieBookingSystem.Api/        # ASP.NET Core backend
│   ├── Controllers/               # API Controllers
│   ├── Models/                    # Database Models
│   ├── Services/                  # Business Logic and Services
│   ├── appsettings.json           # Configuration settings
│   └── Startup.cs                 # Application startup and configuration
├── MovieBookingSystem.Client/     # Angular frontend
│   ├── src/                       # Angular source files
│   ├── app/                       # Angular components, services, and modules
│   └── angular.json               # Angular configuration
└── README.md                      # Project documentation
```

---

## 📄 API Endpoints
Below are some of the key API endpoints for the application:

- **User Authentication**
  - `POST /api/auth/register`: Register a new user.
  - `POST /api/auth/login`: Log in a user.

- **Movies**
  - `GET /api/movies`: Retrieve a list of movies.
  - `GET /api/movies/{id}`: Get details of a specific movie.
  - `POST /api/movies`: Add a new movie (Admin only).

- **Booking**
  - `POST /api/booking`: Book tickets for a selected movie.
  - `GET /api/booking/user/{userId}`: Get all bookings for a specific user.

---


## 📜 License
This project is licensed under the MIT License. See the LICENSE file for details.

---

## 📬 Contact
For questions, suggestions, or contributions, feel free to reach out!

- **GitHub**: [YourUsername](https://github.com/Bikash432)
- **LinkedIn**: [Your LinkedIn Profile](https://www.linkedin.com/in/bikash-thapa-magar-1843a2140/)
