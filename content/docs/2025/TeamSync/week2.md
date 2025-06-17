# Week 2

# Requirements Elaboration

---

## User stories with acceptance criterias

1. As a student, I want to login to the system using Innopolis University SSO, so that I can …
    
    **Acceptance criterias:**
    
2. As a student, I want to create a personal profile with my skills, interests, and past projects so that I can be discovered by project creators or teammates.
    
    **Acceptance criterias:**
    
    - **Given** I’m logged in, **when** I visit the profile page, **then** I can fill in fields name, description, skills, project position, telegram alias, study group, and resume.
    - **Given** I’ve filled out my profile, **when** I return to the profile page, **then** the information is pre-filled and editable.
    - **Given** another user views my profile, **then** they can see a read-only version of my public details.
3. As a student, I want to post a new project with a description and required skills, so that I can find teammates who match my needs.
    
    **Acceptance criterias:**
    
    - **Given** I am logged in and have completed my profile, **when** I click “My projects→Create project,” **then** I see a form with fields: title, description, required skills, status, project link.
    - **Given** I have submitted the form, **then** the project appears in the public project feed.
    - **Given** I return to “My projects”, **then** I can see, edit, or delete my posted project.
4. As a student, I want to receive AI-generated project recommendations based on my skills and preferences, so that I can join relevant and high-fit teams more efficiently.
    
    **Acceptance criterias:**
    
    - **Given** I have completed my profile with skills, interests, and availability, **when** I open the feed, **then** I see a list of projects ranked by relevance to my profile.
    - **Given** I have edited my skills or interests, **when** I open the homepage, **then** the list of suggested projects updates.
5. As a student, I want to apply to projects that match my interests, so that I can participate in projects relevant to my skills and goals.
    
    **Acceptance criterias:**
    
    - **Given** I see a project in the feed, **when** I click “Apply,” **then** I can submit the request.
    - **Given** I applied to a project, **then** I can see my application status in the “My responces” tab.
    - **Given** my application was accepted, **then** I receive a notification and the project appears in “My responces” as “Active.”
6. As a project owner, I want to accept or reject team applications and manage my team members, so that I can control who joins my project and maintain a good team structure.
    
    **Acceptance criterias:**
    
    - **Given** I own a project, **when** someone applies, **then** I see their profile and can click “Accept” or “Reject.”
    - **Given** I accept a student, **then** they appear in my team list.
    - **Given** I view the “Manage Team” section, **then** I can remove members and see their profiles.
7. As a student, I want to see suggestions and filters when browsing projects, so that I can efficiently choose which projects to join.
    
    **Acceptance criterias:**
    
    - **Given** I open the project feed, **then** I see filters like tech stack and tag.
    - **Given** a project closely matches my profile, **then** it is ranked higher or labeled as “Recommended.”
    - **Given** I select filters, **then** only matching projects are shown.
8. As a teacher, I want to login to the system using Innopolis University SSO, so that I can …
    
    **Acceptance criterias:**
    
9. As a teacher, I want to make a page only for my course, so that I can manage the team formation between my students.
    
    **Acceptance criterias:**
    
    - **Given** I am logged in as a professor, **when** I create a course room, **then** students can see/create projects on this board.
    - **Given** students created projects, **then** they can only see and interact with projects from this course.
10. As a teacher, I want to upload the spreadsheet with teams, so that students do not need to write it manually
    
    **Acceptance criterias:**
    
    - **Given** I access the course room dashboard, **when** I upload a CSV/Excel file with team data, **then** the system parses it and creates corresponding projects and team assignments.

# Backlog

---

[🔗 Link to prioritized backlog](https://team-sync-capstone.atlassian.net/jira/software/projects/TS/boards/1?atlOrigin=eyJpIjoiMzBkNTBiMTQ3MWRmNDU1YmJhMzJhZDAxZTE5MjM3NmUiLCJwIjoiaiJ9) 

*if you want to get access to it, log in to Jira with VPN and Innopolis University account*

We have three basic columns in our  board: **“To Do”**, **“In Progress”**, and **“Done”**. Additionally, we’ve added a **“Trashed”** column to store tasks that are no longer relevant.

# Reflection after meeting with TA

---


# Reflection after meeting with Alexey Potemkin

---

- 

# **Project specific progress**

---

## Design

---

## Frontend

---

Links to PRs/Issues for skeleton pages/components.

## Backend

---

Links to PRs/Issues for initial endpoints, link to API documentation.

## ML

---

Summary of research, link to dataset or data collection plan.

# **Weekly commitments**

---

## **Individual contribution of each participant**

| Team member | Contribution |
| --- | --- |
| Diana MInnakhmetova (Lead) |  |
| Danis Sharafiev |  |
| Daria Alexandrova |  |
| Stepan Dementev |  |
| Elizaveta Zagurskih |  |
| Kamilya Shakirova |  |

## **Plan for Next Week**

*...*

**Confirmation of the code's operability**

We confirm that the code in the main branch:

- [ ]  In working condition.
- [ ]  Run via docker-compose (or another alternative described in the `README.md`).