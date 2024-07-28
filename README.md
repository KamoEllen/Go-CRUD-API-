- **Setting Up**: 
  - go get `github.com/gorilla/mux`
  - `go get` is no longer supported outside a module.
  - `go mod init test3` was used at the start of this project

## Architecture Overview

- **Server**: 
  - Runs on `localhost:8000`
  - Uses `gorilla/mux` for routing

- **Data Storage**: 
  - In-memory (slices and maps)
  - No database

- **Routes**:
  - `GET /movies`: List all movies - using /movies to create/add movies 
  - `GET /movies/{id}`: Get movie by ID - using movie id to delete a specific movie 
  - `POST /movies`: Create new movie
  - `PUT /movies/{id}`: Update movie by ID
  - `DELETE /movies/{id}`: Delete movie by ID

- **Testing**:
  -Postman for API endpoint testing
 
