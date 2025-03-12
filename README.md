# First connect to Github Container Registry

## steps to follow to access ghcr.io/openwebui/openwebui:main

Connecting to GitHub Container Registry
To connect, you need to generate a personal access token on GitHub.

Here's how:
Navigate to your Settings > Developer settings > Personal access tokens on GitHub.

Create a new (CLASSIC) token with at least the read:packages scope.
This will allow you to authenticate with the Container Registry using your GitHub credentials.

Using a Personal Access Token (PAT)

To use a PAT, follow these steps:

Generate a Personal Access Token (PAT):
Log in to your GitHub account and navigate to Settings > Developer settings > Personal access tokens.

Click on Generate new token.
Give it a name, for example "Docker GHCR".

Select the read:packages scope (add write:packages if you plan to push images).
Generate the token and copy it (note that you will not be able to retrieve it later).
Authenticating Docker with the PAT:

## Try the connection

Authenticating Docker with the PAT:

In your terminal, run:
docker login ghcr.io -u <your_github_username> -p <your_pat>

Replace <your_github_username> and <your_pat> with your actual GitHub username and PAT.

## CREATE VOLUME in docker

docker volume create open-webui

## RUN CONTAINER

docker compose up -d

Connect on your browser on this url :
http://localhost:3808

# NOTE

Written with the help of llama3B and Chatgpt
