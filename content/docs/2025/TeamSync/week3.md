# Week 3

## **Implemented MVP features**

1. As a student, I want to post a new project with a description and required skills, so that I can find teammates who match my needs.
    
    > Given I am logged in and have completed my profile, when I click “My projects→Create project,” then I see a form with fields: title, description, required skills, status, project link.
    Given I have submitted the form, then the project appears in the public project feed.
    Given I return to “My projects”, then I can see, edit, or delete my posted project.
    > 
    
    **Implemented**
    
    | what is done | PR (link) | Jira task |
    | --- | --- | --- |
    | Authorized user can create a project, choose skills and roles needed, add name, description of the project, optional link to project description.  | [https://github.com/IU-Capstone-Project-2025/team-sync/pull/23](https://github.com/IU-Capstone-Project-2025/team-sync/pull/23) |  |
    |  |  |  |
2. As a student, I want to apply to projects that match my interests, so that I can participate in projects relevant to my skills and goals.
    
    > Given I see a project in the feed, when I click “Apply,” then I can submit the request.
    Given I applied to a project, then I can see my application status in the “My responses” tab.
    > 
    
    **Implemented**
    
    | what is done | PR (link) | Jira task |
    | --- | --- | --- |
    |  |  |  |
    |  |  |  |
    
3. As a student, I want to see suggestions and filters when browsing projects, so that I can efficiently choose which projects to join.
    
    > Given I open the project feed, then I see filters like tech stack and tag.
    > 
    
    **Implemented**
    
    | what is done | PR (link) | Jira task |
    | --- | --- | --- |
    |  |  |  |
    |  |  |  |

## **Demonstration of the working MVP**

*Screenshots/GIFs/PDF presentation/Videos demonstrating the working MVP*

## **ML**

This week, the ML team implemented a basic data migration to test the functionality of both the project and individual microservices [TS-57]. Core classes for interacting with the databases were also developed [TS-55]. We encountered some problems here because there are essential fields which we didn’t have in previous dataset, so we got to lead to a single format. Airflow was integrated for periodic recommendation updates. Additionally, a dummy recommendation service was created [TS-84], and baseline models were added in two parts: Tag-based, including BoW + Cosine similarity [TS-72], and Description-based, using the AllMini-v6 Transformer and Cosine similarity [TS-73]. Also we decided to use KeyDB instead of Redis because it works faster and uses the same clients for connection.

## **Internal demo**

*Notes from internal demo*

Internal Demo & Feedback: Conduct an internal team demo of the current state. Identify bugs and areas for immediate improvement.

# **Weekly commitments**

## **Individual contribution of each participant**

| Team member | Contribution | Jira tasks |
| --- | --- | --- |
| Diana MInnakhmetova (Lead) | Held 2 meetings + 2 with stakeholders + 2 interviews, made design of “create project” and “project feed” | TS-75, TS-76, TS-77, TS-78 |
| Danis Sharafiev | [Dataset synthesis](https://github.com/IU-Capstone-Project-2025/team-sync/pull/17), [add connection with Database](https://github.com/IU-Capstone-Project-2025/team-sync/pull/18), [KeyDB and Airflow containers added](https://github.com/IU-Capstone-Project-2025/team-sync/pull/19), [dummy recommendation system](https://github.com/IU-Capstone-Project-2025/team-sync/pull/25),  | TS-70, TS-71, TS-84, TS-73, TS-87 |
| Daria Alexandrova | [Microsoft entra initialization](https://github.com/IU-Capstone-Project-2025/team-sync/pull/20), [project view page created](https://github.com/IU-Capstone-Project-2025/team-sync/pull/26),  | TS-81, TS-65, TS-82, TS-80 |
| Stepan Dementev | [Initial auth service](https://github.com/IU-Capstone-Project-2025/team-sync/pull/21),  | TS-64, TS-86,  |
| Elizaveta Zagurskih | [Project service created](https://github.com/IU-Capstone-Project-2025/team-sync/pull/23), completed API for resume service,  | TS-58, TS-52, TS-93, TS-94, TS-95, TS-96, TS-97, TS-98 |
| Kamilya Shakirova | Database migrations
(*she was mostly sick and still sick, legal excuse will be provided)* | TS-57 |

## **Plan for Next Week**

### Backend

- Refactoring of the code

### Design

- “Student dashboard” page
- “Onboarding” page
- “Notification” page
- “Favorite projects” page
- “My responses” page

### Frontend

- “My responses” page
- Animations

### ML

- Algorithm enhancement

### Management

- Analysis of interviews and meetings with stakeholders

### CI/CD

- Write unit tests for critical backend logic and frontend components.
- Write integration tests for API endpoints.
- Aim for basic end-to-end tests for the core user journey.
- (ML) Implement basic model validation/testing.
- Deployment

**Confirmation of the code's operability**

We confirm that the code in the main branch:

- [ ]  In working condition.
- [ ]  Run via docker-compose (or another alternative described in the `README.md`).