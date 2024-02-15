# Task-Manager-with-REST-API

A task management web application with a REST API using Django. It allows multiple users to create, view, update, and delete tasks.

## Table of Contents

- [Requirements](#requirements)
- [Installation](#installation)
- [Configuration](#configuration)
- [Environment Variables](#environment-variables)
- [Running the Project](#running-the-project)

## Requirements

- Python (version 3.11.2)
- PostgreSQL (version 15.6)

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Hridoy-31/Task-Manager-with-REST-API.git
   ```

2. Navigate to the project directory:

   ```bash
   cd task_manager
   ```

3. Create and activate a virtual environment:

   ```bash
   python -m venv env
   source env/bin/activate  # For macOS/Linux
   .\env\Scripts\activate    # For Windows
   ```

4. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

## Configuration

1. Set up your database configuration by creating a `.env` file in the project root directory and defining the following variables:

   ```plaintext
   DATABASE_ENGINE=django.db.backends.postgresql
   DATABASE_NAME=your_database_name
   DATABASE_USER=your_database_user
   DATABASE_PASSWORD=your_database_password
   DATABASE_HOST=your_database_host
   DATABASE_PORT=your_database_port
   ```

   Replace `your_database_name`, `your_database_user`, `your_database_password`, `your_database_host` and `your_database_port` with your actual database information.

2. Apply database migrations:

   ```bash
   python manage.py migrate
   ```

## Environment Variables

- **DATABASE_ENGINE**: Specifies the database engine to use. Example value: `django.db.backends.postgresql`.
- **DATABASE_NAME**: The name of the database to connect to.
- **DATABASE_USER**: The username to use when connecting to the database.
- **DATABASE_PASSWORD**: The password to use when connecting to the database.
- **DATABASE_HOST**: The host address of the database server.
- **DATABASE_PORT**: The port number of the database server.

## Running the Project

1. Start the development server:

   ```bash
   python manage.py runserver
   ```

2. Open your web browser and navigate to `http://127.0.0.1:8000/` to view the project.

3. You can now access the project and start working on it!
