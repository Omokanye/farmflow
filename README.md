#  FarmFlow

FarmFlow is a simple application designed to support Nigerian farmers aged 18-45 by providing digital tools to manage their farms efficiently. It addresses challenges like high tech costs, limited internet access, lack of training, and land ownership issues. The app aims to simplify farm operations, track expenses, and promote sustainable agriculture.

###  Objectives
- Facilitate efficient farm management through digital tools.
- Track farming activities using the **Farm Diary**.
- Enhance financial oversight with **Expense Tracking**.
- Provide an accessible platform for sustainable agricultural practices.

---

##  Key Features

### Farm Diary  
- **Dashboard Overview**  
  - Displays recent activities and weather updates.
  - Central hub for adding and managing diary entries.

- **Daily Log Entries**  
  - Forms with date selectors, activity types, and notes.
  - Attachments for relevant photos or files.

- **Calendar View**  
  - Monthly color-coded activities for easy tracking and editing.

### Expense Tracking  
- **Expense Entry Screen**  
  - Simple form to add expenses with categories and notes.
  - Real-time validation to avoid incorrect entries.

- **Summary Dashboard**  
  - Graphical display of expense distribution and trends.

- **Reports and Export Options**  
  - Generate reports in different formats for budgeting.

---

##  Application Overview  
The FarmFlow dashboard serves as the main interface for users. It combines farm management tools with financial tracking. The key components include:

- **Header**: Displays user profile, navigation links, and notifications.
- **Weather Widget**: Provides real-time weather updates.
- **Recent Activities**: Shows recent farm operations.
- **Graphical Insights**: Expense charts with interactive elements.
- **Quick Actions**: Links to add new diary entries or expenses.

---

##  Database Models

1. **Users**
   - `user_id` (Primary Key)  
   - `first_name`, `last_name`, `email`, `password_hash`
   - `location`, `account_type`, `profile_picture`

2. **Farm Diary Entries**
   - `entry_id` (Primary Key)  
   - `user_id` (Foreign Key)  
   - `date`, `activity_type`, `notes`, `attachments`

3. **Expenses**
   - `expense_id` (Primary Key)  
   - `user_id` (Foreign Key)  
   - `date`, `category`, `amount`, `description`

4. **Weather Data**
   - `weather_id` (Primary Key)  
   - `location`, `date`, `temperature`, `conditions`, `humidity`

5. **Educational Resources**
   - `resource_id` (Primary Key)  
   - `title`, `content`, `category`, `resource_link`

6 **Educational Resources**
   - `resource_id` (Primary Key), 
   - `title`, `content`, `category`, `resource_link`

7. **Community Posts and Comments **
   - Posts, `post_id` (Primary Key) `user_id` (Foreign Key)
   - `title`, `content`, `timestamp`

8.**** Comments****
   - `comment_id` (Primary Key)
   - post_id (Foreign Key) user_id (Foreign Key), `content`, `timestamp`

---

##  Relationships
- **Users to Farm Diary Entries**: One-to-Many relationship.  
- **Users to Expenses**: One-to-Many relationship.  
- **Community Posts to Comments**: One-to-Many relationship.

---

##  How to Run the App

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/3mtt-challenge.git

###
Tech Stack
Front-end: HTML, CSS, JavaScript
Back-end: Node.js
Database: MongoDB or SQLite
Version Control: Git & GitHub
