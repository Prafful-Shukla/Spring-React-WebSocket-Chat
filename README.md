# 💬 Real-Time Full-Stack Chat Application

## Project Overview

This is a robust, full-stack application designed to demonstrate real-time, bi-directional communication using modern web technologies. The core of the application is a secure messaging platform built on the reliable **Spring Boot** framework and a responsive user interface powered by **React.js**. It implements the **WebSocket protocol** using **STOMP** and **SockJS** to deliver instant messages between users and across different chat channels.

The platform supports essential chat functionality, including secure user login, a public community chat, and direct private messaging between individuals.

## ✨ Key Features

* **Secure User Authentication:** Implements Registration, Login, and Logout for secure access.
* **Real-Time Messaging:** Instant message delivery using WebSockets.
* **Public Chatroom:** A shared space for group interaction among all online users.
* **Private Messaging:** Send direct, one-on-one messages to specific users.
* **User Management:** Ability to search for and add other users by their username.
* **Message Persistence:** Messages and user data are stored and retrieved from the database.
* **Responsive UI:** Optimized layout for seamless use across desktop and mobile devices.

## ⚙️ Technology Stack

| Category | Technology | Purpose |
| :--- | :--- | :--- |
| **Backend** | **Spring Boot** | Core Java framework for API and WebSocket handling. |
| **Real-Time** | **Spring WebSocket** | Server-side implementation of the WebSocket protocol. |
| **Database** | **MySQL** & **Spring Data JPA** | Relational database persistence and ORM for user/message data. |
| **Frontend** | **React.js** | Library for building the dynamic user interface. |
| **Protocol** | **STOMP & SockJS** | Messaging protocol (STOMP) and reliable client connection (SockJS). |
| **Styling** | **Tailwind CSS** | Utility-first framework for rapid and responsive styling. |
| **Build Tool** | **Maven** | Dependency management and build automation for the Java backend. |

## 🚀 Getting Started

Follow these steps to set up and run the application locally.

### Prerequisites

Ensure you have the following installed on your machine:

* **Java JDK** (v17 or higher recommended)
* **Maven**
* **Node.js** and **npm** or **yarn**
* **MySQL Server**

### 1. Database Setup

1.  Create a new MySQL database instance named `chat` (or another name, but ensure you update the configuration).
2.  Open the `Back-end/src/main/resources/application.properties` file.
3.  Update the database connection details with your credentials:

    ```properties
    spring.datasource.url=jdbc:mysql://localhost:3306/chat
    spring.datasource.username=your_mysql_username
    spring.datasource.password=your_mysql_password
    ```

### 2. Back-end Setup

1.  Navigate to the `Back-end` directory:
    ```bash
    cd Back-end
    ```
2.  Build and run the Spring Boot application using Maven:
    ```bash
    mvn clean install
    mvn spring-boot:run
    ```
    The server should start running on `http://localhost:8080`.

### 3. Front-end Setup

1.  Navigate to the `Front-end` directory:
    ```bash
    cd Front-end
    ```
2.  Install the necessary Node.js dependencies:
    ```bash
    npm install
    # or yarn install
    ```
3.  Start the React development server:
    ```bash
    npm run dev
    # or yarn dev
    ```
    The client application should be accessible at `http://localhost:5173` (or the port specified in your setup).

## 🤝 Contribution

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](link-to-issues-page-if-you-have-one).
