# Async SaaS API Documentation

## Table of Contents
1. [Public API](#public-api)
2. [Team Member API](#team-member-api)
3. [Team Leader API](#team-leader-api)

## Public API
### GET /api/v1/public/get-user
- Description: Returns current authenticated user
- Response:
  ```json
  {
    "user": {
      // User object or null if not authenticated
    }
  }
  ```

### POST /api/v1/public/get-user-by-slug
- Description: Retrieves user by their slug
- Request Body:
  ```json
  {
    "slug": "user-slug"
  }
  ```
- Response:
  ```json
  {
    "user": {
      // User object
    }
  }
  ```

### GET /api/v1/public/invitations/get-team-by-token
- Description: Retrieves team information by invitation token
- Query Parameters:
  - `token`: Invitation token
- Response:
  ```json
  {
    "team": {
      // Team object
    }
  }
  ```

[Rest of the documentation...]