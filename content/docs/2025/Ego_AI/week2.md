# Week 2 

# Detailed Requirements Elaboration

## Updated/detailed user stories

- As a user, I want to chat with the AI in natural language (e.g., "Reschedule my meetings for today") so I can manage tasks conversationally.

- As a user, I want the AI to answer follow-up questions about my schedule (e.g., "What's my next task?") so I can stay informed without checking manually.

- As a user, I want to add or edit tasks by speaking (e.g., "Add a gym session at 6 PM") so I can capture ideas hands-free.

- As a user, I want the AI to transcribe my brainstorming sessions into actionable notes so I can organize ideas faster.

- As a user, I want the AI to automatically shift tasks if I'm running late so my schedule stays realistic.

- As a user, I want the AI to suggest urgent task rescheduling (e.g., "Move this deadline due to low priority") so I can focus on what matters.

- As a user, I want the AI to remind me of habits (e.g., "You usually read at 9 PM") so I can maintain routines.

- As a user, I want the AI to propose breaks based on my productivity patterns so I can avoid burnout.

- As a user, I want the AI to auto-categorize tasks into "To-Do/Doing/Done" columns so I can visualize progress.

- As a user, I want the AI to flag stalled tasks (e.g., "This hasn't moved in 3 days") so I can take action.

- As a user, I want the AI to suggest indoor tasks (e.g., "Work on emails") when bad weather is forecasted so my plans stay flexible.

- As a user, I want the AI to recommend nearby coffee shops for meetings based on my preferences (e.g., "Quiet, with WiFi").

- As a user, I want a weekly report showing my peak productivity hours so I can plan deep work accordingly.

- As a user, I want the AI to compare planned vs. actual task time so I can improve time estimates.

- As a user, I want two-factor authentication for my connected accounts so my data stays secure.

- As a user, I want a free tier with basic features (e.g., task tracking) so I can test the tool before paying.

## Requirements

Based on the user stories and marketing analysis, for the next weeks, we define these requirements:

- Account creation and data saving
- Calendar with tasks (basic CRUD functions)
- AI chat
- Speech-To-Task
- Dynamic rescheduling with AI
- Smart suggestions and reminders
- Kanban board with AI for some projects
- Weather and place recommendations
- Visualization and analytics of user productivity

We've distributed all requirements into weeks:

- **Week 2**
  - Account creation and data saving
  - Calendar with tasks (basic CRUD functions)
  - AI chat
- **Week 3**
  - Speech-To-Task
- **Week 4**
  - Dynamic rescheduling with AI
  - Smart suggestions and reminders 
- **Week 5**
  - Weather and place recommendations
- **Week 6**
  - Visualization and analytics of user productivity

## Project Architecture

![Architecture](https://github.com/setterwars/Capstone-project-2025/blob/main/arch.png?raw=true)

## User flow 

Based on the choosen requirements, we have developed a user flow that will underpin our project.

![User flow](https://github.com/setterwars/Capstone-project-2025/blob/main/user_flow.png?raw=true)

## Prioritized Backlog 

**Link to the backlog**:
https://github.com/orgs/IU-Capstone-Project-2025/projects/1

**Backlog screenshot**:

![Backlog](https://github.com/setterwars/Capstone-project-2025/blob/main/backlog.png?raw=true)

All issues are divided into iterations. In total we have 6 iterations. Also, as you can see, all issues are prioritized in the backlog. The issues have their size indicated to estimate the time needed to complete each task.

# Project-specific progress

## Frontend 

This week we designed the frontend and start develop it.

**Link to the Figma design:** https://www.figma.com/design/zMYnwpNRbPajOsotSTseJR/EGO-AI?node-id=0-1&t=BM9yQnmQUAHViWYA-1

## Backend

In this week In backend side will be realized base CRUD logic and authorization. Also will add connection to the database.

Link to API documentation provided in repository README.md

## ML

- Added voice chat with Whisper 
- implemented chat with LLM

For chat with LLM used **deepseek-r1:1.5b**. For voice model used **tiny** and for embedding used model **mxbai-embed-large**

## DevOps


# Weekly commitments 

## Individual contribution of each participant 

- **Dmitriy Ryazanov**: 

- **Diana Tsoi**: Frontend Design

    **Links:**

    - Link to the Figma design: https://www.figma.com/design/zMYnwpNRbPajOsotSTseJR/EGO-AI?node-id=0-1&t=BM9yQnmQUAHViWYA-1

- **Stepan Sarantsev**: Implemented CRUD (Calendar system), wrote database initializer

    **Links:**

    - Link to commit: https://github.com/IU-Capstone-Project-2025/Ego_AI/commit/939ba7b97afb306da79af3e93c77f46466b5349d

- **Andrey Zhdanov**: Added voice chat with Whisper, implemented chat with LLM, added temporary calendar and vector DB support

    **Links:**
    - Link to commit: https://github.com/IU-Capstone-Project-2025/Ego_AI/commit/7ddf982abdd316508f080808a724794c54909132

- **Artyom Lapin**: 

- **Mikhail Sofin**:

- **Salavat Zaynulin**: Wrote report, created user flow diagram and architecture diagram, backlog creation, work on design

    **Links**
    - Link to the online board: https://excalidraw.com/#room=0a55400de3e2cf3441c6,bBFRwjpDKsK64Lti2_I28A


## Plan for Next Week

Next week we plan to implement these functions:  
  - Speech-To-Task
  - Dynamic rescheduling with AI
  - Smart suggestions and reminders

We also plan to test the parts of the project we've created so far and fix any bugs we find.

## Confirmation of the code's operability

We confirm that the code in the main branch:
- Is in working condition
- Runs via Docker Compose