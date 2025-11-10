# Static Website Deployment Pipeline

This repository contains a **Jenkins Pipeline** for deploying a static portfolio website. The pipeline automates the process of cloning the repository, building (if required), testing (if required), and deploying the static website to your server. It is configured to work with **GitHub webhooks** to automatically trigger the pipeline on push events.

---

## Table of Contents

- [Project Overview](#project-overview)  
- [Features](#features)  
- [Prerequisites](#prerequisites)  
- [Pipeline Stages](#pipeline-stages)  
- [Deployment](#deployment)  
- [Automated Trigger](#automated-trigger)  
- [Folder Structure](#folder-structure)  
- [Contributing](#contributing)  
- [License](#license)  

---

## Project Overview

This project is designed to **automate the deployment** of a static portfolio website using Jenkins. The website is a template downloaded from the internet, and the pipeline ensures it is always deployed to the server whenever there is a new update in the repository.

The pipeline is simple, efficient, and perfect for static websites that do not require a build or test process.

---

## Features

- Automatic deployment of the website to a server directory.
- Triggered automatically via GitHub webhooks on push events.
- Simple, easy-to-read Jenkins pipeline configuration.
- No additional build or test steps required for static content.
- Easily configurable deployment path.

---

## Prerequisites

Before using this pipeline, ensure you have the following:

1. **Jenkins installed** and running on your server.  
2. **Git installed** on the Jenkins host.  
3. **Access to the deployment server** directory where the website will be hosted (e.g., `/var/www/html/`).  
4. **GitHub repository webhook** configured to trigger Jenkins on push events.  

---

## Pipeline Stages

The Jenkins pipeline consists of the following stages:

1. **Clone Repository**  
   - Clones the latest version of the website template from GitHub.

2. **Build**  
   - No build steps are required for static websites. Placeholder for future use.

3. **Test**  
   - No tests are required for static websites. Placeholder for future use.

4. **Deploy**  
   - Copies all website files to the server's web root directory (`/var/www/html/` by default).  
   - You can modify the path in the pipeline if your web server uses a different directory.

---

## Deployment

By default, the pipeline deploys the website to:

```bash
/var/www/html/
