# Project Setup Instructions

Follow the steps below to run the project locally.

### Prerequisites
Ensure you have Node.js and npm installed on your machine. 

### Video Tutorial
You can also follow along with this [video tutorial](https://www.youtube.com/watch?v=xTCBaGeYTck&list=PLnDvRpP8Bnex2GQEN0768_AxZg_RaIGmw&index=22).
1. **Install Node modules**
```bash
npm i
```
## Gernarate key:
2. **Run to generate the key**
 ```bash
node ace generate:key
```

3. **Create .env**
```bash
PORT=3333
HOST=0.0.0.0
NODE_ENV=development
APP_KEY=3HAdSv4l-fRBMiRusUdAo7duVazEshUT => change here => xFrf9LtPHkvzAqACzSDiv088jOZeqsqJ
DRIVE_DISK=local
DB_CONNECTION=sqlite
```

4. **Copy the key generated**
```bash
xFrf9LtPHkvzAqACzSDiv088jOZeqsqJ
  > During development, you may want to set the above secret as "APP_KEY" inside the .env file
```

### Instalations Steps

5. **Install Dependencies ande migrations then run the server:**
```bash
  npm install sqlite3 --save && node ace migration:run && node ace serve
```


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
