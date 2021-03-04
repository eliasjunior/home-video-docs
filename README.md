<!-- PROJECT LOGO -->
<br />
<p align="center">
  <a href="https://github.com/eliasjunior/home-video-api/blob/master/public/movies.png">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Home Video</h3>

  <p align="center">
    It's a web application to play videos on a browser, it's easy to install and setup, access the videos on the phone, computer or anything that has a browser.
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
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project
<p align="center">
    <a href="https://github.com/eliasjunior/home-video-docs/images/design.png">
        <img src="images/design.png" alt="Logo" width="550" height="330">
    </a>
</p>

</br>

Problably there are many great apps to stream video just like this one but I wanted to learn a bit about video streaming,  on the front-end and back-end.

Here's why:
* Build something that I enjoy doing so.
* Apply good code practices because I want flexibility to change and evolve.
* Pray with React and Node.
* I have a bunch of videos on my hard drive and I was curious on how I could build something to access it.


### Built With
* [React](https://reactjs.org/)
* [NodeJs](https://nodejs.org/)


<!-- GETTING STARTED -->
## Getting Started

### Prerequisites

Cheap computer as Raspberry PI or any other computer that you might have.
NodeJs 10 or higher installed on the machine that will run the apps

* Download [NodeJS](https://nodejs.org)  and follow the steps.

### Installation

**Node App**

1. Clone the NodeJs App (back-end)
   ```sh
   git clone https://github.com/eliasjunior/home-video-api.git
   ```
2. Edit .env with your configuration

```properties
REACT_APP_SERVER_HOST=YOUR_MACHINE_IP_ADDRESS
REACT_APP_SERVER_PROTOCOL=http
```
3. Install NPM packages, run the command bellow.
   ```sh
   npm install
   ```
4. More details of the configuration you can find in `src/config.js`   

**React App**

1. Clone the React App (Front-end)
   ```sh
   git clone https://github.com/eliasjunior/home-video.git
   ```
2. Install NPM packages, run the command bellow on both projects in the root folder.
   ```sh
   npm install
   ```
3. More details of the configuration you can find in `src/config.js`

TODO add config sets here!


<!-- USAGE EXAMPLES -->
## Usage

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos work well in this space. You may also link to more resources.

_For more examples, please refer to the [Documentation](https://example.com)_


See the [open issues](https://github.com/othneildrew/Best-README-Template/issues) for a list of proposed features (and known issues).


<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request



<!-- LICENSE -->
## License

Distributed under the MIT License. See `LICENSE` for more information.

