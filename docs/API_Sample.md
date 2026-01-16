# Sample API Documentation

This document provides a sample API reference to demonstrate basic API
documentation structure and style.

## Overview
The Sample User API allows clients to retrieve and manage user information
programmatically.

## Base URL
https://api.example.com/v1

## Authentication
This API uses token-based authentication.

Clients must include an authorization token in the request header:
Authorization: Bearer <your_token>

## Endpoints

### GET /users
Retrieves a list of users.

**Request**
GET /users

**Response**
200 OK
[
{
"id": 1,
"name": "John Doe",
"email": "john@example.com"
}
]

### POST /users
Creates a new user.

**Request**
POST /users
{
"name": "Jane Doe",
"email": "jane@example.com"
}

**Response**
201 Created
{
"id": 2,
"name": "Jane Doe",
"email": "jane@example.com"
}

## Error Codes
- 400 Bad Request – Invalid input
- 401 Unauthorized – Missing or invalid token
- 404 Not Found – Resource not found