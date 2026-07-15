# WildFrame

WildFrame is a full-stack nature photography journal built with React, Spring Boot, and PostgreSQL.

The application allows photographers to upload and organize outdoor photographs, record information about each capture, extract available camera metadata, search their collection, and view geotagged photos on an interactive map.

WildFrame is designed for landscapes, wildlife, birds, plants, insects, macro photography, astrophotography, and other outdoor subjects.

> **Status:** In development

## Live Demo

A public deployment will be added after the first working version is complete.

## Planned Features

* Upload and manage nature photography entries
* Extract available EXIF metadata from uploaded images
* Record titles, categories, locations, dates, and notes
* Browse photos in a responsive gallery
* Search and filter by category, location, date, camera, or lens
* Mark photographs as favorites
* Display geotagged photos on an interactive map
* Edit and delete existing entries

## Technology Stack

### Frontend

* React
* TypeScript
* Vite
* React Router
* React Leaflet

### Backend

* Java 21
* Spring Boot
* Spring Web
* Spring Data JPA
* Maven

### Database and Storage

* PostgreSQL
* Flyway
* Local image storage during development
* Cloud image storage planned for deployment

### Testing and Development

* JUnit 5
* Mockito
* Testcontainers
* Docker Compose
* GitHub Actions

## Architecture

```text
User Browser
     |
     v
React Frontend
     |
     | REST API
     v
Spring Boot Backend
     |
     +-------------------+
     |                   |
     v                   v
PostgreSQL         Image Storage
```

The React frontend handles the gallery, forms, filters, image previews, and interactive map.

The Spring Boot backend handles validation, image uploads, metadata extraction, database operations, and search functionality.

PostgreSQL stores structured photography information, while image files are stored separately.

## Repository Structure

```text
wildframe/
├── backend/
├── frontend/
├── docs/
├── docker-compose.yml
├── .gitignore
└── README.md
```

## Development Roadmap

### Phase 1 — Project Setup

* Initialize the Spring Boot backend
* Initialize the React frontend
* Configure PostgreSQL with Docker Compose
* Connect the frontend to the backend

### Phase 2 — Photography Entries

* Add entry creation, editing, viewing, and deletion
* Add validation and error handling
* Build the gallery and entry detail pages

### Phase 3 — Image Support

* Add image uploads
* Extract EXIF metadata
* Store and display photographs

### Phase 4 — Search and Map

* Add search, filtering, sorting, and pagination
* Display geotagged photos on an interactive map

### Phase 5 — Testing and Deployment

* Add backend and frontend tests
* Configure GitHub Actions
* Deploy the frontend, backend, database, and image storage
* Add screenshots and a live demo link

## Local Development

The planned local services are:

```text
React frontend:  http://localhost:5173
Spring backend:  http://localhost:8080
PostgreSQL:      localhost:5432
```

Detailed setup instructions will be added once the initial project structure is complete.

## Future Improvements

* Multiple photos per entry
* Photography trip collections
* Statistics by camera, lens, category, and location
* Weather information
* Geographic radius search
* Species autocomplete
* AI-assisted subject identification
* User accounts and private galleries
* Location privacy for sensitive subjects

## Author

Created by 2ach as a full-stack Java software engineering portfolio project.
