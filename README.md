<h1 align="center">
  <img src="./assets/dockerize_package_icon.png" alt="icon" width="200"></img>
  <br>
  <b>[Guide] Dockerize Github Projects </b>
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
   -  [:pushpin: Prerequisites](#pushpin-prerequisites)
   -  [Dockerize Github Projects](#dockerize-github-projects)
      -  [Push Docker images manually](#push-docker-images-manually)
         -  [Create Image](#create-image)
            -  [Create a Dockerfile](#create-a-dockerfile)
            -  [Build the image](#build-the-image)
            -  [Push container images to Github Packages (GHCR)](#push-container-images-to-github-packages-ghcr)
         -  [Setting Package](#setting-package)
-  [:world_map: Roadmap](#world_map-roadmap)
-  [:busts_in_silhouette: Contributors](#busts_in_silhouette-contributors)
-  [:sparkles: Credits](#sparkles-credits)
-  [:scroll: License](#scroll-license)
-  [:link: Related Projects](#link-related-projects)
</details>

# :toolbox: Getting Started

## :pushpin: Prerequisites

Before proceeding, make sure you have the following prerequisites installed:

-  Docker: [Install Docker](https://docs.docker.com/get-docker/)
-  Git: [Install Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)

-  Login to `GitHub Container Registry (GHCR)`

   -  Create `Personal Access Token (PAT)` with the `write:packages` and `delete:packages` scopes.

      > For more information, see "[Creating a personal access token](https://docs.github.com/en/github/authenticating-to-github/creating-a-personal-access-token)"

   -  Login to GHCR

      ```sh
      # Export PAT
      export CR_PAT=<personal-access-token>

      # Login to GHCR
      echo $CR_PAT | docker login ghcr.io -u <username> --password-stdin
      ```

## Dockerize Github Projects

### Push Docker images manually

#### Create Image

##### Create a Dockerfile

Create a `Dockerfile` in the root directory of your project. The `Dockerfile` contains instructions for building a Docker image.

Here's a simple example:

```Dockerfile
# Dockerfile
FROM alpine
CMD [ "echo" "Dockerize your Github project"]
```

##### Build the image

Build the Docker image using the `docker build command. Run the following command from the project's root directory:

```sh
docker build -t ghcr.io/<username>/<repository>:<tag> .
```

##### Push container images to Github Packages (GHCR)

```sh
# Tag the image
docker tag <local-image> ghcr.io/<username>/<repository>:<tag>

# Push the image
docker push ghcr.io/<username>/<repository>:<tag>
```

#### Setting Package

-  Public package
-  Connect package to Github Repository
-  Add collaborators
-  Add README instruction

# :world_map: Roadmap

-  [ ] Dockerize Github Projects
   -  [x] Manual
   -  [ ] Using Github Actions
-  [ ] Emoji

# :busts_in_silhouette: Contributors

<a href="https://github.com/QuanBlue/Dockerize-Github-Projects/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=QuanBlue/Dockerize-Github-Projects" />
</a>

Contributions are always welcome!

# :sparkles: Credits

This software uses the following open source packages:

-  [Docker](https://www.docker.com/)
-  [Github](https://github.com/)
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
