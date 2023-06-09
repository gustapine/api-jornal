# 🏴‍☠️ API TIME 🏴‍☠️

## ‼️This repository contains the the project made for n2 server-side class of the 3th semester.‼️

### RESTFUL API  of a newsletter subscribers.

# News Subscribers API Documentation

This documentation provides information about the News Subscribers API, which allows you to manage subscribers' data.

## Base URL

``` http://localhost:3000/api/v1/ ```

## Retrieve All Subscribers

Retrieves information for all subscribers.

- Endpoint: GET ```/assinantes```
- Response Format: JSON
- Response Body:

```json
{
  "data": [
    {
      "cpf": "123.456.789-00",
      "nome": "Fulano de Tal",
      "email": "fulano@example.com"
    },
    {
      "cpf": "987.654.321-00",
      "nome": "Beltrana Silva",
      "email": "beltrana@example.com"
    },
    ...
  ]
}
```
## Retrieve Subscriber by ID

Retrieves information for a specific subscriber by their ID.

- Endpoint: GET ```/assinantes/:id```
- Parameters:
- id: The ID of the subscriber
- Response Format: JSON
- Response Body:

```json
{
  "data": {
    "cpf": "123.456.789-00",
    "nome": "Fulano de Tal",
    "email": "fulano@example.com"
  }
}
```
## Create Subscriber

Creates a new subscriber:

- Endpoint: POST ```/assinantes```
- Request Format: JSON
- Request Body:

```json
{
  "cpf": "123.456.789-00",
  "nome": "Fulano de Tal",
  "email": "fulano@example.com"
}
```
- Response Format: JSON
- Response Body:

```json
{
  "data": {
    "cpf": "123.456.789-00",
    "nome": "Fulano de Tal",
    "email": "fulano@example.com"
  }
}
```
## Update Subscriber

Updates the information for a specific subscriber by their ID.

- Endpoint: PUT ```/assinantes/:id```
- Parameters:
-  id: The ID of the subscriber
- Request Format: JSON
- Request Body:

```json
{
  "cpf": "123.456.789-00",
  "nome": "Fulano de Tal",
  "email": "fulano@example.com"
}
```

- Response Format: JSON
- Response Body:

```json
{
  "data": {
    "cpf": "123.456.789-00",
    "nome": "Fulano de Tal",
    "email": "fulano@example.com"
  }
}

```
## Delete Subscriber

Deletes a specific subscriber by their ID.

- Endpoint: DELETE ```/assinantes/:id```
- Parameters:
- id: The ID of the subscriber
- Response Format: JSON
- Response Body:

```json
{
  "data": {
    "cpf": "123.456.789-00",
    "nome": "Fulano de Tal",
    "email": "fulano@example.com"
  }
}
```
## Retrieve Subscriber E-mail by ID

Retrieves email information for a specific subscriber by their ID.

- Endpoint: GET ```/assinantes/email/:id```
- Parameters:
- id: The ID of the subscriber
- Response Format: JSON
- Response Body:

```json
{
  "data": {
    "nome": "Fulano de Tal",
    "email": "fulano@example.com"
  }
}
```
## Retrieve Subscriber E-mail by E-mail

Retrieves email information for a specific subscriber by their e-mail.

- Endpoint: GET ```/assinantes/email/esc/:email```
- Parameters:
- e-mail: The e-mail of the subscriber
- Response Format: JSON
- Response Body:

```json
{
  "data": {
    "nome": "Fulano de Tal",
    "email": "fulano@example.com"
  }
}
```

```bash
Feel free to copy and paste this Markdown format directly into your README.md file on GitHub.

I hope this helps!
```
