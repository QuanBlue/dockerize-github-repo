<h1 align="center">
  <img src="./assets/dockerize_package_icon.png" alt="icon" width="200"></img>
  <br>
  <b>Dockerize Github Projects </b>
</h1>

<p align="center">Containerize code repository using Docker to simplify deployment, improve portability, and streamline development workflows.</p>

<!-- Badges -->
<p align="center">
  <a href="https://github.com/QuanBlue/Dockerize-Github-Projects/graphs/contributors">
    <img src="https://img.shields.io/github/contributors/QuanBlue/Dockerize-Github-Projects" alt="contributors" />
  </a>
  <a href="">
    <img src="https://img.shields.io/github/last-commit/QuanBlue/Dockerize-Github-Projects" alt="last update" />
  </a>
  <a href="https://github.com/QuanBlue/Dockerize-Github-Projects/network/members">
    <img src="https://img.shields.io/github/forks/QuanBlue/Dockerize-Github-Projects" alt="forks" />
  </a>
  <a href="https://github.com/QuanBlue/Dockerize-Github-Projects/stargazers">
    <img src="https://img.shields.io/github/stars/QuanBlue/Dockerize-Github-Projects" alt="stars" />
  </a>
  <a href="https://github.com/QuanBlue/Dockerize-Github-Projects/issues/">
    <img src="https://img.shields.io/github/issues/QuanBlue/Dockerize-Github-Projects" alt="open issues" />
  </a>
  <a href="https://github.com/QuanBlue/Dockerize-Github-Projects/blob/main/LICENSE">
    <img src="https://img.shields.io/github/license/QuanBlue/Dockerize-Github-Projects.svg" alt="license" />
  </a>
</p>

<p align="center">
  <b>
      <a href="https://github.com/QuanBlue/Dockerize-Github-Projects">Documentation</a> •
      <a href="https://github.com/QuanBlue/Dockerize-Github-Projects/issues/">Report Bug</a> •
      <a href="https://github.com/QuanBlue/Dockerize-Github-Projects/issues/">Request Feature</a>
  </b>
</p>

<br/>

<details open>
<summary><b>📖 Table of Contents</b></summary>

-  [:toolbox: Getting Started](#toolbox-getting-started)
   -  [Push a image to Github Packages (GHCR)](#push-a-image-to-github-packages-ghcr)
   -  [Use Github Actions to Publish a Docker image to Github Packages (GHCR)](#use-github-actions-to-publish-a-docker-image-to-github-packages-ghcr)
   -  [:pushpin: Prerequisites](#pushpin-prerequisites)
   -  [:hammer_and_wrench: Installation](#hammer_and_wrench-installation)
-  [:world_map: Roadmap](#world_map-roadmap)
-  [:busts_in_silhouette: Contributors](#busts_in_silhouette-contributors)
-  [:sparkles: Credits](#sparkles-credits)
-  [:scroll: License](#scroll-license)
-  [:link: Related Projects](#link-related-projects)
</details>

# :toolbox: Getting Started

Push a image to Github Packages (GHCR)

## Push a image to Github Packages (GHCR)

1. Create image
2. Create PAT on Github
3. Authenticate GHCR
4. Tag and push our image to GHCR

```sh
export CR_PAT=<TOKEN>
echo $CR_PAT | docker login ghcr.io -u USERNAME --password-stdin
```

## Use Github Actions to Publish a Docker image to Github Packages (GHCR)

1. Create repo - and Checkin our Dockerfile
2. Build your Github action workflow
3. Trigger our workflow

## :pushpin: Prerequisites

-  **Python:** `>= 3.10.7`
-  **Docker Engine:** Docker provides a consistent and portable environment for running applications in containers. Install [here](https://www.docker.com/get-started/).

To run this project, you need to add the following environment variables to your `.env` file in `/`:

-  **App configs:** Create `.env` file in `./`

   -  `SECRET_KEY`: a key used by Flask to encrypt and sign session data.
   -  `PORT`: specify which port the Flask application should listen on.

   Example:

   ```sh
   # .env
   SECRET_KEY="Readme-template"
   PORT=3000
   ```

You can also check out the file `.env.example` to see all required environment variables.

> **Note**: If you want to use this example environment, you need to rename it to `.env`.

## :hammer_and_wrench: Installation

To clone and run this application, you'll need [Git](https://git-scm.com) and [Python](https://www.python.org/downloads/) installed on your computer. From your command line:

```bash
# Clone this repository
git clone https://github.com/QuanBlue/Dockerize-Github-Projects

# Go into the repository
cd Readme-template

# Install dependencies
npm install

# Run the app
npm start
```

> **Note**
> If you're using Linux Bash for Windows, [see this guide](https://www.howtogeek.com/261575/how-to-run-graphical-linux-desktop-applications-from-windows-10s-bash-shell/) or use `node` from the command prompt.

# :world_map: Roadmap

-  [x] Update theme
-  [x] Emoji
-  [ ] Add more features

# :busts_in_silhouette: Contributors

<a href="https://github.com/QuanBlue/Dockerize-Github-Projects/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=QuanBlue/Dockerize-Github-Projects" />
</a>

Contributions are always welcome!

# :sparkles: Credits

This software uses the following open source packages:

-  [Node.js](https://nodejs.org/)
-  [Marked - a markdown parser](https://github.com/chjj/marked)
-  Emojis are taken from [here](https://github.com/arvida/emoji-cheat-sheet.com)

# :scroll: License

Distributed under the MIT License. See <a href="./LICENSE">`LICENSE`</a> for more information.

# :link: Related Projects

-  <u>[**QuanBlue**](https://github.com/QuanBlue/QuanBlue)</u>: My bio
-  <u>[**Portfolio**](https://github.com/QuanBlue/Portfolio)</u>: My first portfolio website, using MERN stack. [Visit here](https://quanblue.netlify.app/)
-  <u>[**Readme-template**](https://github.com/QuanBlue/Dockerize-Github-Projects)</u>: A template for creating README.md

---

> Bento [@quanblue](https://bento.me/quanblue) &nbsp;&middot;&nbsp;
> GitHub [@QuanBlue](https://github.com/QuanBlue) &nbsp;&middot;&nbsp; Gmail quannguyenthanh558@gmail.com
