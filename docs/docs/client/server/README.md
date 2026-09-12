# Server

This directory contains the backend part of the project.

## Responsibilities

- REST API development
- Business logic
- Data validation
- Database communication
- Authentication and security
- Communication with the frontend

## Planned Technology

- Python
- Flask
- REST API
- SQLite / Database

## API Architecture

The frontend client will communicate with the server
through HTTP/REST API endpoints.

```text
Client
   |
   | HTTP Request
   v
Flask Server
   |
   | Database Operations
   v
Database
