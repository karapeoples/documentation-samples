##Troll Hub — API Reference

## Base URL
`/api`

## Authentication
If an endpoint requires authentication, include the bearer token:
`Authorization: Bearer <token>`

## Schemas

### User
- firstName (string)
- lastName (string)
- email (string)
- country (string)
- password (string)

### Comment
- name (string)
- comment (string)
- score (string)

## Endpoints

### Auth
| Endpoint | Method | Description |
|---|---:|---|
| /auth/register | POST | Register a user and return token |
| /auth/login | POST | Login and return token |

### Users
| Endpoint | Method | Description |
|---|---:|---|
| /newUser | GET | Get list of users |
| /newUser/:id | GET | Get a user by ID |
| /newUser/:id | PUT | Update a user |
| /newUser/:id | DELETE | Delete a user |
| /newUser/:id/favorites | GET | Get a user's favorites |

### Comments
| Endpoint | Method | Description |
|---|---:|---|
| /comments | GET | Get all comments |
| /comments/user_comments/:name | GET | Get comments for a user |

### Favorites
| Endpoint | Method | Description |
|---|---:|---|
| /favorites/:id | GET | Get a favorite by ID |
| /favorites | POST | Save a comment to favorites |
| /favorites/:favorites_id | DELETE | Delete a favorite |
