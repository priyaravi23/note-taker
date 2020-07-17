## Note Taker

*Create an application that can be used to write, save, and delete notes. This application will use an express backend and save and retrieve note data from a JSON file*

### Description

- Build the backend for a given frontend application
- The following HTML routes should be created:
    - GET `/notes` - Should return the notes.html file.
    - GET `*` - Should return the index.html file
    
- The application should have a db.json file on the backend that will be used to store and retrieve notes using the fs module
- The following API routes should be created:
    - GET `/api/notes` - Should read the db.json file and return all saved notes as JSON
    - POST `/api/notes` - Should receive a new note to save on the request body, add it to the db.json file, and then return the new note to the client
    - DELETE `/api/notes/:id` - Should receive a query parameter containing the id of a note to delete

### User Story

```text
AS A user, I want to be able to write and save notes
I WANT to be able to delete notes I've written before
SO THAT I can organize my thoughts and keep track of tasks I need to complete
```

### Acceptance Criteria

```text
Application should allow users to create and save notes.
Application should allow users to view previously saved notes.
Application should allow users to delete previously saved notes.
```