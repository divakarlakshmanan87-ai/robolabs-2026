# AI Mastery
### Tutor, Creator, Worker
#### Divakar Lakshmanan an AI Enthusiast
I design systems, architect them, identify solutions which will help the guest needs

## Hook
Raise Your hand if,
1. Used ChatGPT?
2. Asked AI to do homework?
3. Generated an image?
4. Built an app?
5. Automated something?

By the end of the session,
every one of you will know how to build something with AI.

---
## AI as TUTOR
### I. Traditional Classroom VS AI Tutor
### Traditional Classroom
- Teacher explains
- Student takes notes
- Student memorizes
### ✅ AI Tutor
- Explains simply
- Uses analogies
- Draws diagrams
- Creates quizzes
- Generates flashcards
- Adapts to your learning style

### II. Prompt Engineering
Effective AI tutoring begins with prompt engineering—knowing what and how to ask.
Different Prompting techniques,
### 1. RTF Prompt (Role, Task, Format)
- Role: Define who the AI should act as
- Task: Clearly describe what the AI must do
- Format: Specify output structure, constraints, and style
### 2. COSTAR Prompt (Context, Objective, Style, Example, Task, Action)
- Context: Relevant background information
- Objective: Goal you want to achieve
- Style: Tone and format preferences
- Example: Desired output sample
- Task: Specific action required
- Action: Next steps or execution plan
### 3. COT (Chain of Thoughts)
### 4. Advanced Prompt (6-Part Framework)
- Persona: Expert identity for the AI
- Task: Clear, specific action needed
- Format: Output structure and constraints
- Example: Sample of desired output
- Context: Background to guide the AI
- Tone: Writing style and voice

### Tryouts (Prompting)
1. BASIC QUESTION (Weak)
```
Create a study guide for biology.
```
2. RTF PROMPT (Role, Task, Format)
```
Act as a high school biology teacher. 
Create a study guide for photosynthesis that includes key terms, processes, and 5 practice questions. 
Format it as a numbered list with bold headings.
```
What you will see,
1. ❌ Too vague | No direction | Generic output
2. ✓ Clear role | Specific task | Defined format

### III. Custom GPTs or GEMS (reusable prompts)
SYSTEM INSTRUCTIONS:
```
You are an expert Study Tutor AI designed to help students learn effectively, not just get answers.

### 🎯 Your Goals:
- Help users deeply understand concepts
- Break down complex topics into simple explanations
- Encourage active learning, not passive reading
- Adapt explanations based on the user’s level

### 🧑‍🏫 Your Teaching Style:
- Explain like a great teacher (clear, simple, structured)
- Use analogies, real-world examples, and step-by-step breakdowns
- Ask guiding questions instead of giving direct answers immediately (Socratic method when useful)
- Adjust difficulty (beginner, intermediate, advanced) based on the user

### 📚 What You Should Do:
1. Ask what the user already knows before teaching
2. Explain concepts in small chunks (avoid overload)
3. Give examples after every explanation
4. Provide short summaries at the end
5. Offer practice questions or mini quizzes
6. Help with homework, but don’t just give answers — guide thinking
7. If user asks for direct answer, give it but include explanation

### 🧩 Teaching Framework:
For each topic:
- Step 1: Text book definition
- Step 2: Simple explanation (ELI5 if needed)
- Step 3: Slightly deeper explanation
- Step 4: Real-world example
- Step 5: Quick recap
- Step 6: 2–3 practice questions

### 🗣️ Interaction Rules:
- Be friendly, patient, and encouraging
- Never shame the user for not knowing something
- If user is confused, re-explain in a different way
- Keep responses clear and not too long unless asked

### 🎓 Personalization:
- Ask for:
  - Subject
  - Topic
  - Level (school, college, beginner, etc.)
  - Goal (exam prep, concept clarity, quick revision)

### 📝 Output Format:
- Use headings and bullet points
- Highlight key points
- Keep explanations structured and easy to scan

### 🚫 Avoid:
- Overly technical jargon without explanation
- Long paragraphs without structure
- Giving answers without teaching the reasoning

### 💡 Bonus Features:
- Provide memory tricks / mnemonics when useful
- Give quick revision notes on request
- Create flashcards if asked
```
### IV. RAG system (Notebooklm)
```
https://notebooklm.google.com/
```
---
## AI as CREATOR
### I. Build a Second Brain (Using Claude Code)
| RAG                                    | LLM Wiki                            |
| -------------------------------------- | ---------------------------------------------- |
| Retrieves information at question time | Builds knowledge during ingestion              |
| Searches raw documents                 | Searches a curated wiki                        |
| Same work repeated for every query     | Work compounds over time                       |
| Vector database + embeddings           | Markdown pages + links                         |
| Best for huge document collections     | Best for growing personal/team knowledge bases |

### Use the second-brain SKILL.md file
### SKILL.md = Tools
- Specific capabilities I can use
- Here's a hammer, here's how to use it
- Focused on what I can do
### claude.md = System Instructions
- Core rules about how I should behave
- Be honest, be helpful, respect privacy
- Focused on who I am and how I act

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
### Add an AI Study Buddy feature to the existing StudySprint web application.
```
Add an AI Study Buddy feature to the existing StudySprint web application.

Purpose:
The AI Study Buddy should help students in grades 8–11 decide what to study, organize their available time, and understand school topics.

Use the Gemini API through secure server-side code.

Do not expose the Gemini API key in frontend code.
Store the API key using the AI Studio Secrets feature.

Create a page and dashboard widget called:

“Ask Study Buddy”

The student can type questions such as:

- What should I study first?
- I only have 30 minutes. Make me a plan.
- Help me prepare for my Biology quiz.
- Explain why this task is important.
- Create a quiz for this topic.
- Make flashcards from my notes.

Use the logged-in student’s active tasks as context.

For study-plan questions, consider:

- Due date
- Priority
- Difficulty
- Estimated study time
- Current task status
- Student’s available time

Return structured JSON using this format:

{
  "summary": "Short recommendation",
  "sessions": [
    {
      "taskId": "task id when available",
      "title": "Task title",
      "subject": "Subject",
      "durationMinutes": 25,
      "reason": "Why this task was selected",
      "priority": "High"
    }
  ],
  "remainingTasks": [],
  "encouragement": "Short positive message"
}

Display the response as attractive study-session cards rather than raw JSON.

Each recommendation card should show:

- Subject
- Task title
- Recommended duration
- Priority
- Reason
- Start Study button
- Add to Plan button

Add these quick-action buttons:

- Plan My Evening
- What Should I Do First?
- Quiz Me
- Explain a Topic
- Create Flashcards

For Quiz Me:

- Ask for the subject and topic
- Generate five age-appropriate questions
- Ask one question at a time
- Wait for the student’s answer
- Provide a hint before revealing the correct answer
- Show the final score

For Explain a Topic:

- Ask for grade level and topic
- Use simple language
- Provide a real-world analogy
- Give one example
- Ask one question to check understanding

For Create Flashcards:

Return:

{
  "flashcards": [
    {
      "front": "Question or term",
      "back": "Answer or explanation"
    }
  ]
}

Add loading indicators, friendly error messages, and retry behavior.

Do not allow the AI to complete graded homework or write a full essay for the student.

When asked to provide direct homework answers, respond by offering:

- a hint
- a step-by-step explanation
- a similar practice problem

Use a fast Gemini model suitable for interactive web-app responses.

Build and test the complete feature.
```
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
---
## AI as WORKER
### I. Demo using n8n (Workflow automation tool)
n8n is a workflow automation tool that lets you connect different apps and services together to automate repetitive tasks without coding.

---
## Pre-REquisite / Setup

```
1. https://gemini.google.com/ - Free Account
2. https://notebooklm.google.com/ - Free Account
3. https://claude.ai/ - Can be installed with Pro plan only (Not a mandatory but only if possible)
4. Claude desktop -  claude.ai/download
5. https://aistudio.google.com/ - Free Account
6. https://lovable.dev/ - Free Limit Account
7. https://obsidian.md/ - Free Account
```
