### II. Build a Student Planner via Google AI Studio
```
Build a responsive web app called “StudySprint”.

Purpose:
StudySprint helps students in grades 8–11 organize homework, quizzes, tests, and projects into a realistic daily study schedule.

Target users:
Middle-school and high-school students in the United States.

Design:
- Clean, modern, friendly student-focused design
- Mobile-first and also optimized for laptops
- Bright but professional appearance
- Rounded cards and large readable text
- Simple icons for subjects, deadlines, difficulty, breaks, and completion
- Do not make the interface feel childish
- Include a light and dark mode
- Use accessible contrast and keyboard-friendly controls

Main screen:
Display the heading:
“Turn your assignments into a smart study plan.”

Display the subtitle:
“Tell us what you need to finish and how much time you have.”

Create these inputs:

1. Grade level
   - Grade 8
   - Grade 9
   - Grade 10
   - Grade 11

2. Available study date
   - Default to today

3. Preferred start time
   - Example: 4:00 PM

4. Total available study time
   - 30 minutes
   - 60 minutes
   - 90 minutes
   - 2 hours
   - Custom

5. Preferred study method
   - Short focused sessions
   - Longer deep-focus sessions
   - Balanced

Task entry section:
Allow the student to add multiple tasks.

Each task must include:
- Task name
- Subject
- Task type: Homework, Quiz, Test, Essay, Project, Reading, Other
- Due date
- Difficulty: Easy, Medium, Hard
- Estimated time in minutes
- Importance: Normal, Important, Critical

Include common subject options:
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

Allow students to:
- Add a task
- Edit a task
- Delete a task
- Duplicate a task

Smart planning behavior:
When the student clicks “Create My Study Plan,” generate a realistic timeline.

Prioritize tasks using:
1. Closest deadline
2. Highest importance
3. Highest difficulty
4. Estimated completion time
5. Available study time

The generated plan must:
- Never exceed the student’s available time
- Split large assignments into smaller sessions
- Include 5–10 minute breaks
- Put urgent tasks earlier
- Avoid scheduling only difficult subjects back-to-back
- Include a short reason for each priority decision
- Clearly show unfinished tasks that could not fit today

Example output:

4:00–4:25 PM
Algebra Homework
Reason: Due tomorrow and marked Important

4:25–4:35 PM
Break

4:35–5:05 PM
Biology Quiz Review
Reason: Test is approaching and difficulty is Hard

5:05–5:20 PM
English Essay Outline
Reason: Starting early reduces last-minute work

Generated-plan screen:
Show the schedule as a visual timeline.

Each study block must include:
- Start and end time
- Subject
- Task name
- Duration
- Priority reason
- Complete checkbox
- Edit button
- Remove button
- Add to Calendar button

Also include:
- Overall progress bar
- Total study time
- Total break time
- Number of completed tasks
- “Regenerate Plan” button
- “Start Study Session” button
- “Add Entire Plan to Google Calendar” button

Study-session mode:
Create a simple focus timer.
- Show the current task
- Countdown timer
- Pause, resume, and complete buttons
- Show the next task
- Display a positive message after completing a task

Data storage:
For the first version, use browser local storage so the app works without requiring an account.

Save:
- Tasks
- Generated plans
- Completion status
- Student preferences

AI behavior:
Use AI only to help organize and explain the plan.
The app must not complete homework or provide test answers.

When generating the plan, return structured data containing:
- startTime
- endTime
- title
- subject
- durationMinutes
- type
- priority
- reason
- isBreak

Error handling:
- Require at least one task
- Prevent negative study durations
- Warn when a deadline has already passed
- Warn when available study time is too short
- Never create overlapping study blocks
- Show friendly error messages

Include sample data so the app can be demonstrated immediately:
1. Algebra worksheet, due tomorrow, Medium, 30 minutes
2. Biology quiz review, due in 2 days, Hard, 40 minutes
3. English essay outline, due in 5 days, Medium, 20 minutes

Build the complete working first version.
```
