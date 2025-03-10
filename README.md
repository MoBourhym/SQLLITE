# SQLite CRUD Application

A simple Android application demonstrating basic CRUD (Create, Read, Update, Delete) operations using SQLite database.

![UI](UI.png)

## Features

- Add new users to the database
- View all users in a list
- Update existing user information
- Delete users from the database
- Simple and intuitive user interface

## Project Structure

The application consists of the following components:

1. **MainActivity**: Main activity that handles the UI and user interactions.
2. **DBHandler**: Database helper class that manages SQLite operations.
3. **SQLite Database**: Local database for storing user information.

## Implementation Details

### Database Structure

The application uses a simple SQLite database with a single table:

- **Table Name**: Users
- **Columns**:
  - `id` (INTEGER): Primary key, auto-incremented
  - `name` (TEXT): User's name

### CRUD Operations

- **Create**: Add a new user with a name
- **Read**: View all users in a ListView
- **Update**: Select a user from the list and modify their name
- **Delete**: Remove a user from the database

## How to Use

1. **Add User**:
   - Enter the user's name in the text field
   - Click the "Save" button

2. **View Users**:
   - All users are displayed in the ListView

3. **Update User**:
   - Select a user from the list
   - Their name will appear in the text field
   - Modify the name
   - Click the "Update" button

4. **Delete User**:
   - Select a user from the list
   - Click the "Delete" button

## Technical Implementation

The application uses:

- `SQLiteOpenHelper` for database operations
- `ContentValues` to insert and update data
- `Cursor` to retrieve data from the database
- `ArrayAdapter` to display data in the ListView
- `AdapterView.OnItemClickListener` to handle item selections

## Requirements

- Android Studio
- Minimum SDK: API 21 (Android 5.0 Lollipop)
- Target SDK: API 33 (Android 13)

## Installation

1. Clone the repository
2. Open the project in Android Studio
3. Build and run the application on an emulator or physical device

## Future Enhancements

- Add more user fields (email, phone, etc.)
- Implement search functionality
- Add confirmation dialogs for update and delete operations
- Improve UI with material design components
- Add user authentication
