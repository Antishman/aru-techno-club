# ARU Techno Club Website

## Overview

The ARU Techno Club Website is a dynamic, full-stack web application designed to showcase the club's activities, manage events, and handle user registrations. It features a modern, responsive frontend built with HTML, CSS (Tailwind), and JavaScript, coupled with a robust backend powered by Node.js, Express, and SQLite.

## Features

- 🎨 Responsive, neumorphic design with dark mode toggle
- 📅 Dynamic event display and management
- 👥 User registration system
- 🔐 Admin panel with secure authentication
- 📊 User data management
- 🌐 RESTful API for frontend-backend communication

## Technologies Used

- Frontend:
  - HTML5
  - CSS3 (Tailwind CSS)
  - JavaScript (ES6+)
- Backend:
  - Node.js
  - Express.js
  - SQLite
- Authentication:
  - JSON Web Tokens (JWT)
  - bcrypt for password hashing

## Prerequisites

Before you begin, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14.0.0 or later)
- npm (usually comes with Node.js)

## Installation

1. Clone the repository:
   
   git clone https://github.com/antishman/aru-techno-club.git
   cd aru-techno-club
   

2. Install the dependencies:
   
   npm install
   

3. Start the server:
   
   node server.js
   

4. Open your web browser and navigate to `http://localhost:3000`

## Project Structure


aru-techno-club/
├── public/
│   └── index.html
├── server.js
├── database.sqlite
├── package.json
└── README.md


## API Endpoints

- POST `/api/register`: Register a new user
- GET `/api/events`: Retrieve all events
- POST `/api/admin/login`: Admin login
- POST `/api/admin/events`: Add a new event (protected)
- GET `/api/admin/users`: Retrieve all users (protected)

## Admin Access

To access the admin panel:
1. Click on the "Admin" button in the footer
2. Use the following credentials:
   - Username: admin
   - Password: admin123

**Note:** Change these credentials after the first login for security purposes.

## Customization

- To modify the frontend, edit the `public/index.html` file
- Backend logic can be adjusted in `server.js`
- Database schema changes should be made in the `db.serialize()` function in `server.js`

## Security Considerations

- Use environment variables for sensitive information (e.g., JWT secret)
- Implement rate limiting for API endpoints
- Use HTTPS in a production environment
- Regularly update dependencies to patch security vulnerabilities

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).

## Support

For support, please open an issue in the GitHub repository or contact the maintainers.



Developed with ❤️ by the ARU Techno Club team
