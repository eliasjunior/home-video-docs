[![Tests](https://github.com/eliasjunior/home-video/actions/workflows/tests.yml/badge.svg)](https://github.com/eliasjunior/home-video/actions/workflows/tests.yml)
<br />
<p align="center">
  <a href="https://github.com/eliasjunior/home-video-api/blob/master/public/movies.png">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Home Video</h3>

  <p align="center">
  Home Video is a small self-hosted web app for streaming videos from your own computer through the browser.
  It was built as a learning project to explore how video streaming, file organization, and a simple full-stack React + Node.js setup work together.
    <br />
    <br />
  </p>
</p>

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#technical-overview">Technical overview</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
<p align="center">
    <a href="https://github.com/eliasjunior/home-video-docs/blob/main/images/design.png">
        <img src="images/design.png" alt="Logo" width="100%" height="100%">
    </a>
</p>

</br>


Home Video is a hobby project built to better understand the fundamentals of browser-based video streaming and full-stack JavaScript development.

The goal was not to build a production media server, but to explore how the core pieces fit together:

	•	Serving video files from a local machine
	•	Streaming media through a Node.js backend
	•	Building a responsive UI with React
	•	Organizing a simple media library structure

The app makes it possible to browse and play personal video files from any device on the local network using only a browser.

### Built With
* [React](https://reactjs.org/) - [Front-end App](https://github.com/eliasjunior/home-video)
* [NodeJs](https://nodejs.org/) - [Back-end App](https://github.com/eliasjunior/home-video-api)


<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

Cheap computer as Raspberry PI or any other computer that you might have.
NodeJs 10 or higher installed on the machine that will run the apps

* Download [NodeJS](https://nodejs.org)  and follow the steps.

### Installation(Production environment)

<li><a href="https://github.com/eliasjunior/home-video-api" target="_blank">Node App</a></li>

1. Clone the NodeJs App (back-end)
    ```sh
    git clone https://github.com/eliasjunior/home-video-api.git
    ```

2. Edit .env with your configuration

    ```properties
    SERVER_HOST=YOUR_MACHINE_IP_ADDRESS
    SERVER_PROTOCOL=http
    SERVER_PORT=8080
    IMG_FOLDER_FALL_BACK=/Images
    VIDEO_PATH=Absolute videos path
    MOVIES_DIR=Movies folder
    SERIES_DIR=Series folder
    VIDEO_PATH_LOCAL=Local path, for development
    IMG_FOLDER_FALL_BACK= leave it blank if you don't want the app to read video/images from another folder
    ```

3. More details of the configuration you can find in `src/config.js`  

4. The folder's structure must follow the structure below, images and subtitles at the same folder.

    <a href="https://github.com/eliasjunior/home-video-docs/blob/main/images/files-structure.png">
            <img src="images/files-structure.png" alt="Logo"  width="300px" height="200px">
    </a>


5. Install NPM packages, run the command bellow.
    ```sh
    npm install
    ```

6. Run app    
 ```sh
   npm start
 ```
<li><a href="https://github.com/eliasjunior/home-video" target="_blank">React App</a></li>

1. Clone the React App (Front-end)
    ```sh
    git clone https://github.com/eliasjunior/home-video.git
    ```

2. Edit .env with your configuration   
    ```properties
    REACT_APP_SERVER_HOST=YOUR_SERVER_IP_ADDRESS
    REACT_APP_SERVER_PROTOCOL=http
    ```

3. More details of the configuration you can find in `src/config.js`  

4. Install NPM packages.
    ```sh
      npm install
    ```

5. Build the App
    ```sh
      npm run build
    ```

6. Run app    
    ```sh
      npm start
    ```
## Usage

Mobile 

<p align="center">
    <a href="https://github.com/eliasjunior/home-video-docs/blob/main/images/home.png">
        <img src="images/home.png" alt="Logo" width="200px" height="350px">
    </a>
    <a href="https://github.com/eliasjunior/home-video-docs/blob/main/images/list.png">
        <img src="images/list.png" alt="Logo" width="200px" height="350px">
    </a>
    <a href="https://github.com/eliasjunior/home-video-docs/blob/main/images/list-search.png">
        <img src="images/list-search.png" alt="Logo" width="200px" height="350px">
    </a>
</p>
<p align="center">
    <a href="https://github.com/eliasjunior/home-video-docs/blob/main/images/player.png">
        <img src="images/player.png" alt="Logo" width="736px" height="414px">
    </a>
</p>

Desktop
<p align="center">
    <a href="https://github.com/eliasjunior/home-video-docs/blob/main/images/desktop.png">
        <img src="images/desktop.png" alt="Logo" width="100%" height="100%">
    </a>
    <a href="https://github.com/eliasjunior/home-video-docs/blob/main/images/desktop-list.png">
        <img src="images/desktop-list.png" alt="list"  width="100%" height="100%">
    </a>
    <a href="https://github.com/eliasjunior/home-video-docs/blob/main/images/desktop-list-search.png">
        <img src="images/desktop-search.png" alt="list" width="100%" height="100%">
    </a>
</p>
<!-- Technical -->

## Technical overview

<li><a href="https://github.com/eliasjunior/home-video" target="_blank">React App</a></li>

### Frameworks and Libs

Front-End (React)

The front-end is a small React application focused on simplicity and responsiveness.
	•	Component-based structure for reusability
	•	Responsive layout for both mobile and desktop
	•	Basic search and browsing experience
	•	Styling written with plain CSS using BEM methodology
	•	Flexbox used for layout structure
	

<li><a href="https://github.com/eliasjunior/home-video" target="_blank">Server App</a></li>

The back-end is a lightweight Node.js server responsible for discovering media files and streaming them to the browser.
	•	REST API for listing available media
	•	Basic HTTP video streaming support
	•	File-system based media organization (movies, series, images, subtitles)
	•	Environment-based configuration for flexible local setups

<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.
