# medbikriTask
type "npm install" in the project directory after cloning it to install all the packages.
To start the server: node server.js, server starts on port 5000
To view the video details : visit "localhost:5000/videos"

Data is obtained from youtube API every 10 seconds and then stored in the local mongodb server.
When GET request is made to the page "localhost:5000/videos", data stored in the database is obtained and then sent as response to the get request made
Before the next request is sent to the youtube API, previous data from the server is deleted and the new data is stored in their place so that we have the latest data and we do not run out of storage.
