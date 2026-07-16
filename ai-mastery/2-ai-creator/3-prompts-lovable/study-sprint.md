### III. Build a Student Planner via Lovable
```
Build a modern AI-powered Study Planner web application called “StudySprint”.

The app should use a Kanban board layout and include authentication, a database, and secure user-specific data.

1. Authentication

- Users can sign up using email and password.
- Users can log in and log out.
- Keep users signed in between sessions.
- Each user must only be able to view and manage their own study tasks.
- Use Supabase authentication and database.
- Include:
  - Sign-up page
  - Login page
  - Forgot-password flow
  - Logout button
- Redirect authenticated users to the dashboard.
- Redirect unauthenticated users to the login page.

2. Study Task Management

Users can create, edit, delete, and duplicate study tasks.

Each study task should contain:

- Task title
- Subject
- Description
- Task type
- Priority
- Difficulty
- Due date
- Estimated study time
- Status
- Created date
- User ID

Subject options:

- Math
- Biology
- Chemistry
- Physics
- English
- U.S. History
- World History
- Computer Science
- Foreign Language
- Other

Task type options:

- Homework
- Quiz
- Test
- Essay
- Project
- Reading
- Revision
- Other

Priority options:

- Low
- Medium
- High
- Critical

Difficulty options:

- Easy
- Medium
- Hard

Status options:

- To Study
- In Progress
- On Hold
- Completed

3. Kanban Study Board

Create four Kanban columns:

- To Study
- In Progress
- On Hold
- Completed

Display each task as a card.

Each task card should show:

- Task title
- Subject
- Due date
- Priority
- Difficulty
- Estimated study time
- Task type

Users must be able to drag and drop tasks between columns.

When a task is moved, update its status in the database immediately.

Use clear visual labels for:

- Priority
- Difficulty
- Overdue status
- Completed status

4. Smart Study Planner

Add a button called:

“Create My Study Plan”

When clicked, ask the student for:

- Study date
- Preferred start time
- Total available study time
- Preferred study style

Study style options:

- Short focused sessions
- Longer deep-focus sessions
- Balanced

Generate a recommended study schedule using the student’s active tasks.

Prioritize tasks using:

1. Closest due date
2. Highest priority
3. Highest difficulty
4. Estimated study time
5. Task status

The generated study plan should:

- Never exceed the available study time
- Put urgent tasks first
- Split large tasks into smaller study sessions
- Include short breaks
- Avoid placing multiple difficult subjects back-to-back
- Explain why each task was prioritized
- Clearly show tasks that could not fit in the schedule

5. Generated Study Plan View

Display the generated study plan as a timeline.

Each study block should show:

- Start time
- End time
- Subject
- Task title
- Duration
- Priority reason
- Completion checkbox

Include:

- Total study time
- Total break time
- Number of study sessions
- Number of tasks completed
- Regenerate Plan button
- Save Plan button

Save generated study plans in the database and associate them with the logged-in user.

6. Dashboard

Display summary cards for:

- Total Tasks
- Completed Tasks
- Pending Tasks
- Overdue Tasks
- Total Planned Study Time

Also display:

- Upcoming deadlines
- Recently completed tasks
- Tasks due this week
- Progress percentage

Add filters for:

- Subject
- Priority
- Difficulty
- Due date
- Status

Add a search box for finding tasks.

7. Calendar-Ready Feature

Add an “Add to Calendar” button for each planned study session.

Also add:

“Add Entire Plan to Calendar”

For the first version, generate a downloadable calendar file using the .ics format.

The calendar event should include:

- Event title: [Subject] — [Task title]
- Start date and time
- End date and time
- Description
- Priority
- Study reason
- Reminder 10 minutes before

Do not require direct Google Calendar integration in the first version.

Make the app architecture ready for Google Calendar OAuth integration later.

8. Database

Automatically create the required Supabase tables.

Create tables for:

Profiles:
- id
- email
- full_name
- grade_level
- created_at

Study tasks:
- id
- user_id
- title
- description
- subject
- task_type
- priority
- difficulty
- due_date
- estimated_minutes
- status
- created_at
- updated_at

Study plans:
- id
- user_id
- plan_date
- start_time
- available_minutes
- study_style
- total_study_minutes
- total_break_minutes
- created_at

Study sessions:
- id
- study_plan_id
- user_id
- task_id
- title
- subject
- start_time
- end_time
- duration_minutes
- reason
- is_break
- is_completed
- created_at

Create all relationships automatically.

9. Security

Enable Supabase Row Level Security.

Ensure:

- Users can only read their own tasks
- Users can only create tasks linked to their own user ID
- Users can only update their own tasks
- Users can only delete their own tasks
- Users can only view their own study plans and study sessions

Never expose service-role keys in frontend code.

Use secure authenticated database queries.

10. Design

Create a modern SaaS-style student dashboard.

Design requirements:

- Clean and professional
- Friendly for students in grades 8–11
- Responsive on laptops and phones
- Light and dark mode
- Rounded cards
- Clear typography
- Accessible contrast
- Smooth drag-and-drop interactions
- Simple subject icons
- Progress bars
- Professional sidebar navigation

Navigation should include:

- Dashboard
- Kanban Board
- Study Planner
- Calendar
- Profile
- Logout

Do not make the design childish.

11. Sample Data

After a new user signs up, optionally allow them to load sample tasks:

- Algebra worksheet
  - Due tomorrow
  - Priority: High
  - Difficulty: Medium
  - Estimated time: 30 minutes
  - Status: To Study

- Biology quiz review
  - Due in 2 days
  - Priority: Critical
  - Difficulty: Hard
  - Estimated time: 40 minutes
  - Status: To Study

- English essay outline
  - Due in 5 days
  - Priority: Medium
  - Difficulty: Medium
  - Estimated time: 25 minutes
  - Status: In Progress

12. Validation and Error Handling

- Require a task title
- Require a subject
- Require a due date
- Prevent negative study durations
- Warn when a due date has passed
- Prevent overlapping study sessions
- Show friendly error messages
- Show loading indicators
- Show success notifications
- Confirm before deleting a task

Build the complete deploy-ready application.

Use only the components, database tables, authentication logic, and dependencies required for this app.
Do not add social features, messaging, payments, or unnecessary admin functionality.
```
