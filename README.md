# Labguy - Open-Source CMS for Multimedia Artists

**Labguy** is an open-source content management system designed for multimedia artists, developed by [@jakubkanna](https://twitter.com/jakubkanna) 👨‍🔬.

What started as a simple student project to create a blog API turned into a nearly one-year journey of researching the best solution for creating a Content Management System (CMS) suitable for artists.

Although I don't consider it to be 'the best,' I believe it offers an interesting alternative for those looking for a CMS that supports various types of media (3D, sound, video, high-quality images), is fast, and offers good scalability.

## Architecture

Labguy consists of three main applications, all written in TypeScript:
- **Client**
- **Dashboard**
- **REST API**

## How It Works

Labguy uses a hosted **Express server** in conjunction with **Prisma** and **JSON Web Tokens (JWT)** to process CRUD requests from the Dashboard and GET requests from the Client.

### Dashboard

The **Dashboard** is built with:
- React
- @mui/material
- react-router-dom
- tinymce
- @rjsf/core
- material-react-table

The Dashboard is ready to be hosted on GitHub, with automatic sync and deployment using GitHub Actions.

### REST API

The **REST API** relies on:
- Express
- Prisma
- Cloudinary
- Multer

It does feature Deployment action.

### Client

The **Client** is built individually. There is no predefined pattern, as it is best to create a personalized front-end application that follows the design rules set by the design. Labguy-client is just a boilerplate you might start with.

## Inspiration

Examples of the Client can serve as inspiration for design and usage, showcasing how to integrate the various features and media types Labguy supports.
