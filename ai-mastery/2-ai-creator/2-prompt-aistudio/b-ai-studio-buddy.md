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
