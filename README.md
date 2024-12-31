# Labguy - Open-Source CMS for Multimedia Artists

[![Deploy to Sever](https://github.com/jakubkanna/labguy-server/actions/workflows/deploy.yml/badge.svg)](https://github.com/jakubkanna/labguy-server/actions/workflows/deploy.yml) [![Sync Fork and Deploy to GitHub Pages](https://github.com/jakubkanna/labguy-dashboard/actions/workflows/sync.yml/badge.svg)](https://github.com/jakubkanna/labguy-dashboard/actions/workflows/sync.yml)

What started as a simple student project to create a blog API turned into a nearly one-year journey of researching the best solution for creating a Content Management System (CMS) suitable for artists.

Although I don't consider it to be 'the best,' I believe it offers an interesting alternative for those looking for a CMS that supports various types of media (3D, sound, video, high-quality images), is fast, and offers good scalability.

## Architecture

Labguy consists of three main applications, all written in TypeScript:
- **Client**
- **Dashboard**
- **REST API**

You can find the code for each part in the respective repositories:

- [**Labguy Dashboard**](https://github.com/jakubkanna/labguy-dashboard.git)
- [**Labguy Client**](https://github.com/jakubkanna/labguy-client.git)
- [**Labguy Server (REST API)**](https://github.com/jakubkanna/labguy-server.git)

## How It Works

Labguy uses a **Express server** in conjunction with **Prisma** and **JSON Web Tokens (JWT)** to process CRUD requests from the Dashboard and GET requests from the Client. It's self-hosted and doesn't require any third party. 

### Dashboard

The **Dashboard** is built with:
- React
- @mui/material
- react-router-dom
- tinymce
- @rjsf/core
- material-react-table

The Dashboard is ready to be hosted on GitHub, with automatic sync and deployment using GitHub Actions.

- [**Labguy Dashboard Repository**](https://github.com/jakubkanna/labguy-dashboard.git)

### REST API

The **REST API** relies on:
- Express
- Prisma
- Cloudinary
- Multer

It also includes deployment actions for automatic updates.

- [**Labguy Server (REST API) Repository**](https://github.com/jakubkanna/labguy-server.git)

### Client

The **Client** is built individually. There is no predefined pattern, as it is best to create a personalized front-end application that follows the design rules set by the project. **Labguy-client** serves as a boilerplate to get started.

- [**Labguy Client Repository**](https://github.com/jakubkanna/labguy-client.git)

## Inspiration

Examples of the Client can serve as inspiration for design and usage, showcasing how to integrate the various features and media types Labguy supports.

- https://jakubkanna.github.io/jakubkanna-client/
- https://insidewww.github.io/insidejob-client

## Screenshots

![Screenshot 1](assets/Screenshot%202024-12-29%20at%2018.34.58.png)
![Screenshot 2](assets/Screenshot%202024-12-29%20at%2018.35.30.png)
![Screenshot 3](assets/Screenshot%202024-12-29%20at%2018.35.47.png)
