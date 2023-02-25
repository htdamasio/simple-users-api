# simple-users-api

A very basic API made with Node.js from scratch 

## Features
- Create User
- Update User
- Delete User
- List Users

Added the identification of query parameters and path parameters

## Installation & Set Up
1. Clone the project
```sh
git clone git@github.com:htdamasio/simple-users-api.git
```

2. Install dependencies
```sh
npm install
```

3. Run for development
```sh
npm run dev
```

## Usage

### Create User
Use a POST method on your API client for the route `http://localhost:3333/users` sending a the information in the request body 
```json
{
  "name": "Jhon Doe",
  "email": "jhondoe@email.com"
}
```

### Update User
Use a PUT method on your API client for the route `http://localhost:3333/users/:id` sending the id through route params and other information in the request body 
```json
{
  "name": "Jhon Doe Updated",
  "email": "jhondoeupdated@email.com"
}
```

### Delete User
Use a DELETE method on your API client for the route `http://localhost:3333/users/:id` sending the id through route params

### List Users
Use a DELETE method on your API client for the route `http://localhost:3333/users`. You can use query parameters to filter the results, the one avaiable is `search`, so it will look something like `http://localhost:3333/users?search=jhon`
