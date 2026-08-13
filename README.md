# WINGSPAN

## Project Overview
Wingspan is a centralized image library and REST API built for Reiman Gardens at Iowa State
University. Each semester, senior design and capstone teams are given projects that involve
building applications using Reiman Gardens' butterfly and insect photo collection. Without a
centralized system, each team rebuilds image storage from scratch, manually updates photos
when content changes, and duplicates files across multiple projects, resulting in unnecessary
storage costs and inconsistent content.

Wingspan solves this by providing a single hosted platform where Nathan Brockman at Reiman
Gardens uploads and manages butterfly and insect photos through an admin dashboard. Student
teams access that content through API keys tied to their project and semester.

## Tech Stack  
Backend: Java Spring Boot 3.2.1, Maven, package fs3.wingspan
Frontend: Vite, Handlebars, TypeScript, Bootstrap 5
Database: PostgreSQL on DigitalOcean
File Storage: DigitalOcean Spaces (S3 compatible)
Server: DigitalOcean Droplet

## Access / Documentation
Wingspan is up at http://159.203.134.226/ 

The application is only accessible to authorized staff and senior design groups. Please visit https://seniord.cs.iastate.edu/2026-March-16/ for detailed reports and demos of the final app. 

If you go to Project Artifacts then Final Report, this is a detailed report of an overview of the project, design choices, work completed, results, and the appendix. Progress demos are also v=available under Progress Reports. Thank you!

## To Run Locally
Required: Java 17, Maven, Node.js and npm, local PostgreSQL instance

Backend: Create a local application.properties file at src/main/resources/application.properties with your local database credentials and DigitalOcean Spaces credentials from Nathan. Open WingspanApplication in IntelliJ and run.

Frontend: cd into the frontend directory, run npm install then npm run dev.

