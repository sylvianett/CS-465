# Travlr Getaways – Full Stack Web Application

**Course:** CS 465 – Full Stack Development  
**Author:** Sylvia Davis  

---

## Project Overview

Travlr Getaways is a full stack web application built using the MEAN stack (MongoDB, Express, Angular, Node.js). The application serves both a customer-facing website and an administrative single-page application (SPA).

Customers can view available trips, while administrators can securely log in to manage trip data through protected endpoints.

This final iteration includes authentication and route protection to secure administrative functionality.

---

## Technologies Used

- MongoDB (NoSQL Database)
- Express.js (Backend Framework)
- Angular (Frontend SPA)
- Node.js (Server Runtime)
- Mongoose (MongoDB ODM)
- JSON Web Tokens (JWT) for Authentication

---

# Module Eight Reflection

## Architecture

This project used two types of frontend development approaches. The customer-facing side utilized Express with server-rendered HTML templates, while the administrative side used an Angular single-page application (SPA).

Server-rendered HTML relies on the backend to dynamically generate full pages before sending them to the browser. In contrast, the Angular SPA updates content dynamically without refreshing the entire page by consuming RESTful API endpoints.

The SPA approach provides a smoother and more modern user experience, while the Express-rendered approach is simpler and efficient for content-based pages. Working with both helped me understand the advantages and trade-offs of each model.

The backend used MongoDB, a NoSQL database, because it stores data in flexible, JSON-like documents. Since the application was built using JavaScript technologies across the stack, MongoDB integrates naturally with the environment. Its schema flexibility also allowed for easier updates to the Trip model during development.

---

## Functionality

JSON (JavaScript Object Notation) is a data format used for transmitting structured data, while JavaScript is a programming language. JSON does not contain logic or functions—it strictly represents data.

In this application, JSON serves as the bridge between frontend and backend. The backend API returns trip data in JSON format, and the Angular frontend consumes that data to dynamically render UI components.

During development, I refactored code multiple times to improve efficiency and maintainability. I separated route logic into controllers, modularized API calls, and reused Angular components for trip listings and administrative forms.

The benefits of reusable UI components include:
- Reduced code duplication
- Improved readability
- Easier debugging
- Consistent user interface design
- Faster feature implementation

Refactoring improved the overall structure and scalability of the application.

---

## Testing

The application uses RESTful API endpoints that correspond to HTTP methods such as GET, POST, PUT, and DELETE. Each endpoint handles specific operations related to trip data.

Testing involved verifying that each endpoint responded correctly and returned appropriate status codes. After implementing authentication, testing required additional validation to ensure:

- Login credentials were properly validated
- Tokens were generated upon successful authentication
- Protected endpoints were inaccessible without a valid token
- Administrative routes were properly secured

Adding security introduced an additional layer of complexity because errors could occur in authentication logic, token handling, or route protection.

This process strengthened my understanding of endpoint structure, API security, and full stack integration.

---

## Reflection

This course significantly enhanced my understanding of full stack web development. I moved beyond building isolated frontend or backend components and learned how to integrate them into a cohesive, secure system.

Key skills developed in this course include:

- Designing RESTful APIs
- Structuring applications using the MVC pattern
- Building single-page applications (SPA)
- Connecting Angular to backend APIs
- Implementing MongoDB schemas with Mongoose
- Adding authentication and route protection
- Refactoring for scalability and maintainability

Completing this project aligns directly with my professional goal of transitioning into a software engineering role. Building a fully functional and secure full stack application has strengthened both my technical abilities and my confidence as a developer.

This project represents my ability to design, build, secure, and test a complete web application using industry-relevant technologies.
