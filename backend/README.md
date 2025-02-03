# API Documentation

## Overview

This document outlines the API endpoints for managing groups, to-do lists, and tasks in the backend server.

## Base URL

```
/api/
```

## Group Endpoints

### Retrieve all groups

**GET** `/api/group/`

- Retrieves all group information.

### Retrieve a specific group

**GET** `/api/group/<id>`

- Retrieves the specific group information based on the given ID.

### Add a new group

**POST** `/api/group/`

- Adds a new group.

### Update a group

**PUT** `/api/group/<id>/`

- Updates the group information (e.g., renaming the group).

### Delete all groups

**DELETE** `/api/group/`

- Deletes all groups and all associated to-do lists.

### Delete a specific group

**DELETE** `/api/group/<id>`

- Deletes a specific group and all its associated to-do lists.

### Delete all to-do lists in a group

**DELETE** `/api/group/<id>/list`

- Deletes all to-do lists from a group but keeps the group information.

### Add a new to-do list to a group

**POST** `/api/group/<id>/list`

- Adds a new to-do list to the specified group.


## To-Do List Endpoints

### Retrieve all to-do lists

**GET** `/api/list/`

- Retrieves all to-do lists, regardless of group.

### Retrieve a specific to-do list

**GET** `/api/list/<id>`

- Retrieves the information of a specific to-do list.

### Update a to-do list

**PUT** `/api/list/<id>`

- Updates a specific to-do list.

### Delete a to-do list

**DELETE** `/api/list/<id>`

- Deletes a specific to-do list.


## Task Endpoints

### Add a new task to a to-do list

**POST** `/api/list/<id>/task/`

- Adds a new task to the specified to-do list.

### Update a specific task in a to-do list

**PUT** `/api/list/<id>/task/<id>`

- Updates a specific task within a specified to-do list.

### Delete all tasks from a to-do list

**DELETE** `/api/list/<id>/task/`

- Deletes all tasks from a specific to-do list.

### Delete a specific task from a to-do list

**DELETE** `/api/list/<id>/task/<id>`

- Deletes a specific task from a specific to-do list.

---

This document will be updated as the API evolves. Let us know if any changes or improvements are needed!

