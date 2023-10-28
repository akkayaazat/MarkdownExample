# MarkdownExample
# User Management Screen Specification

## Overview
This document details the specifications for the User Management Screen. Tailored for administrators and those with user management permissions, this interface offers a comprehensive platform to seamlessly manage user accounts. With a dual-pane layout, administrators can view a list of users and their details simultaneously.

## UI Components

### Left Pane: User List

#### Buttons
- **+ New User**: Initiates the process to create a new user. Clicking this button clears all existing data from the right pane, providing a blank slate for the new user's information.
- **Hide Disabled User**: Functions as a toggle switch. When toggled on, any users with their "Enabled" status set to "false" are immediately hidden from view, streamlining the user list.

#### User Table
- **Columns**: 
  - ID: A unique identifier for each user.
  - User Name: The name the user utilizes for logging in.
  - Email: The user's email address.
  - Enabled: Indicates if a user account is active or not.
  
- **Functionality**: Each row offers an interactive snapshot of individual user details. A single click on any row instantly populates the right pane with the selected user's comprehensive details.

### Right Pane: User Details

#### Header
- **New User**: This header is prominently displayed when the administrator is in the process of adding a new user.

#### Form Fields
- **Username**: An alphanumeric input field where the desired username is entered.
- **Display Name**: A field intended for the user's full name or nickname.
- **Phone**: Designed exclusively for phone numbers, ensuring proper format.
- **Email**: A validation-enabled field for the accurate input of email addresses.
- **User Roles**: A dropdown selection offering multiple roles: Guest, Admin, Super-Admin. This allows for defining access levels.
- **Enabled**: A checkbox. Marking this sets the user's status as active.

#### Button
- **Save User**: A vital function. Clicking this button commits the details entered or edited in the right pane. New users are appended to the user list, while updated details of existing users are seamlessly saved.

## Behavior & Interactions

1. **Initial Load**: The maiden launch of the page showcases a comprehensive user list. The right pane, in anticipation of its next task, presents itself in the "New User" mode, awaiting data input.
  
2. **Adding a New User**: 
   - Initiate by clicking the **+ New User** button.
   - Populate necessary details in the right pane.
   - Conclude by clicking **Save User**. This action integrates the new user into the existing list.
  
3. **Editing an Existing User**: 
   - Begin by selecting a desired user from the list.
   - In the right pane, proceed to modify the necessary details.
   - Ensure changes are retained by clicking **Save User**.
  
4. **Hiding Disabled Users**: 
   - The **Hide Disabled User** button serves as a visual filter. Toggling it on will remove non-active users from the list, offering a more streamlined view to the administrator.
