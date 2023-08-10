# Student IA Allocation System

Welcome to the Student IA Allocation project! This web-based system is designed to facilitate the allocation of student instructional assistants (IA) based on available rooms and student credentials. The system is developed using PHP, HTML, and MySQL.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Database Schema](#database-schema)
- [Contributing](#contributing)
- [License](#license)

## Introduction

The Student IA Allocation System aims to streamline the process of assigning instructional assistants to various classrooms while taking into consideration student credentials. This system provides an efficient way to manage IA allocation and optimize resource utilization.

## Features

- **Room Allocation**: The system allocates students to available rooms based on the room's capacity and other criteria.

- **Credential Matching**: Students are allocated to rooms in a way that maximizes the match between their credentials and the required credentials for each room.

- **User-friendly Interface**: An intuitive web interface allows administrators to manage room information, student credentials, and perform IA allocations.

- **Data Persistence**: All data is stored in a MySQL database, ensuring that the allocation information is stored securely and can be retrieved when needed.

## Requirements

To run this project locally, you'll need:

- Web server (e.g., Apache)
- PHP 7.0 or higher
- MySQL database
- Git (optional)

## Installation

1. Clone the repository to your local machine:
   ```bash
   git clone https://github.com/isa/student-ia-allocation.git
   ```

2. Configure your web server to serve the project from the cloned directory.

3. Import the provided MySQL database dump (`database_dump.sql`) into your MySQL server:
   ```bash
   mysql -u isa -p isa < database_dump.sql
   ```

## Usage

1. Access the system through your web browser by entering the appropriate URL.

2. Use the administrator interface to manage room information, student credentials, and perform IA allocations.

3. Follow the on-screen instructions to allocate students to rooms based on available capacity and credential match.

## Database Schema

The database schema includes the following tables:

- `rooms`: Stores information about available rooms, including room ID, capacity, and required credentials.

- `students`: Contains student details such as student ID, name, and credentials.

- `allocations`: Tracks the allocation of students to rooms, including the allocation ID, room ID, and student ID.

## Contributing

Contributions to this project are welcome! Feel free to open issues or pull requests if you'd like to enhance the system's functionality, fix bugs, or suggest improvements.

## License

This project is licensed under the [MIT License](LICENSE).

---
