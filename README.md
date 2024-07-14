# Project Setup Instructions

Follow the steps below to run the project locally.

### Prerequisites
Ensure you have Node.js and npm installed on your machine. 

### Video Tutorial
You can also follow along with this [video tutorial](https://www.youtube.com/watch?v=xTCBaGeYTck&list=PLnDvRpP8Bnex2GQEN0768_AxZg_RaIGmw&index=22).


### Steps

1. **Install Dependencies:**
   ```bash
   npm install && npm install sqlite3 --save && node ace migration:run && node ace serve
``

### Checking API Functionality with Postman

To verify if the API is functioning correctly using Postman:

1. Ensure that the local server is running.
2. In Postman, send a GET request to the endpoint `http://localhost:3333/api/moments`.
3. If the API is working correctly, you will receive a response with JSON data. For example:
   ```json
   {
       "data": [
           // Your data here
       ]
   }
4. If the API is functioning properly, the response will contain data within the `data` array. If you receive `data: []`, it indicates that the API is operational but currently has no registered moments.

This method allows you to easily check if the API is responding correctly using Postman with the specified endpoint.
