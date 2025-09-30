# Taxi Reservation System 🚕

http://googleusercontent.com/image_generation_content/0

A comprehensive Java project demonstrating the system design and object-oriented principles behind a modern taxi booking application. This project focuses on building a scalable and maintainable architecture for a ride-hailing service.

[![Java Version](https://img.shields.io/badge/java-8+-blue.svg)](https://www.java.com)
[![Build Tool](https://img.shields.io/badge/Build-Apache%20Ant-red)](https://ant.apache.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

## 📋 Project Overview

The Taxi Reservation System is a backend application that simulates the core logic of a ride-sharing service. It's designed to showcase clean code, robust architecture, and the practical application of design patterns. The primary goal is not to create a polished UI, but to build a strong foundation that could be extended into a full-fledged desktop or web application.

## 🏛️ System Design & Architecture

This project is built with a component-based architecture, focusing on the separation of concerns.

#### Core Components:
* **Booking Service:** The central component that manages the entire lifecycle of a ride request, from matching a rider with a driver to finalizing the trip.
* **Location Service:** Responsible for tracking and updating the real-time locations of all drivers.
* **User Management:** Handles the profiles and data for both Riders and Drivers.
* **Database:** A conceptual layer for storing user data, ride history, and system state.

#### Object-Oriented Design:
The system is modeled using clear, object-oriented principles with classes such as:
* `User`, `Rider`, `Driver`: Representing the actors in the system.
* `Ride`: An object containing all details of a single trip (e.g., start/end location, fare, status).
* `Vehicle`: Represents the driver's car details.

#### Design Patterns Applied:
* **Singleton Pattern:** Used for the `BookingManager` to ensure a single, globally accessible instance controls all ride assignments.
* **Strategy Pattern:** Implemented for fare calculation, allowing for different pricing models (e.g., standard, peak-hour, long-distance) to be swapped easily.
* **Observer Pattern:** Used to notify different parts of the system about status changes in a `Ride` (e.g., notify billing when a ride is completed).

## ✨ Features

* **User & Driver Registration:** Onboard new riders and drivers to the system.
* **Ride Booking:** Allow riders to request a trip from a pickup point to a destination.
* **Driver Matching:** Automatically finds the nearest available driver for a ride request.
* **Fare Calculation:** Dynamically calculates the ride fare based on distance and pricing strategy.
* **Trip Management:** Track the status of a ride (Requested, In-Progress, Completed, Canceled).

## 🛠️ Technology Stack

* **Language:** **Java**
* **Build System:** **Apache Ant**
* **Core Concepts:** Object-Oriented Programming, System Design Principles, Data Structures, Design Patterns.

## 🚀 Getting Started

This project is built as a standard Java application and can be run from any machine with the Java Development Kit (JDK).

#### Prerequisites:
* JDK 8 or higher
* Apache Ant

#### Installation & Execution:
1.  **Clone the repository:**
    ```sh
    git clone [https://github.com/your-username/taxi-reservation-system.git](https://github.com/your-username/taxi-reservation-system.git)
    ```
2.  **Navigate to the project directory:**
    ```sh
    cd taxi-reservation-system
    ```
3.  **Build the project using Ant:**
    This will compile the source files and create an executable `.jar` file in the `/dist` directory.
    ```sh
    ant
    ```
4.  **Run the application:**
    ```sh
    java -jar dist/TaxiReservationSystem.jar
    ```

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.
