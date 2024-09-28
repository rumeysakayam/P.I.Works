# P.I.Works
User interface specification document for technical assignment.

## Overview
This document outlines the user interface specifications for the User Management Screen. This screen will enable administrators to manage user accounts, including viewing, creating, editing, and deleting user information.

## Requirements
1. **User List Display**: The screen should display a list of all users in a tabular format.
2. **Search and Filter Functionality**: Users should be able to search for specific users by name or email and filter the user list by enabled status (true/false).
3. **Create New User**: A button to create a new user will be available.
   
## UI Components

### 1. +New User Button
- **Label**: "+ New User"
- **Behavior**: Clicking this button opens a modal or form to fill in new user details.

### 2. New User Form
This form includes the following fields:
- **Username**: 
  - **Input Type**: Text
  - **Placeholder**: "Enter username"
  
- **Display Name**: 
  - **Input Type**: Text
  - **Placeholder**: "Enter display name"
  
- **Phone Number**: 
  - **Input Type**: Text
  - **Placeholder**: "Enter phone number"

- **Email**: 
  - **Input Type**: Text
  - **Placeholder**: "Enter email"

- **User Role**: 
  - **Input Type**: Dropdown
  - **Options**: "Guest", "Admin", "Super Admin"

- **Enabled Checkbox**: 
  - **Label**: "Enabled"
  - **Behavior**: A checkbox that indicates whether the user account is active.
    
### 3. Save User Button
- **Label**: "Save User"
- **Behavior**: Clicking this button will save the new user information and close the modal/form. Validation should ensure all fields are filled correctly.

### 4. User List Table
- **Columns**:
  - **ID**: 
    - **Class**: Unique identifier, auto-incrementing by one.
  - **Username**: Displayed as a link or text.
  - **Email**: Displayed as text.
  - **Enabled**: Displayed as true/false.
  
- **Sorting and Filtering**:
  - The table should support sorting by ID, Username, and Email.
  - A filter option should allow users to view only enabled or disabled accounts.

### 5. Hide Enabled Users Checkbox
- **Label**: "Hide Enabled Users"
- **Behavior**: A checkbox that, when checked, hides all users with an enabled status. When unchecked, all users will be visible.

