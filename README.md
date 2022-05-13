# Arcadia coding challenge
This pages describes the coding challange for the full stack developer role in engineering architecture at Airbus Defence and Space.

## Objectives
The objectives of this challenge is to assess:
- your capabilities for coding and software design
- how you use technologies to solve a problem
- your coding style and its documentation

## Scoring
You will be scored according to the following criteria:
- Reliability of code
- Code style and documentation
- Performance efficiency of application
- Maintinability of code

## Challange - Company Employees

Create a website that allows to assign employees to companies with a great UX. To manage the employees and companies 
implement a backend service with a database. To fill your database with entries implement a client to retrieve the employees and users from the `https://random-data-api.com/`.
The challenge is spilt into three parts for backend, frontend and DevOps. You can implement the backend and the frontend in the language of you choice.
You may use frameworks or libraries like Angular or React to create the web application. FYI: We use spring boot and angular in our stack.

## Backend

The backend service shall provide a client to retrieve companies and users from the `https://random-data-api.com/` and store them
in a database of your chooise (in memory database is also fine).



```
https://random-data-api.com/api/company/random_company
https://random-data-api.com/api/users/random_user
```
To load and access the data implement a Restful API to:
- Load a given number of users(employees) or companies from the `https://random-data-api.com/` (basic properties are sufficient)
- Get the stored employees and companies
- Create relations between employees and companies (an employee can only be assigned to one company)

**Optional**

- CRUD operations for the employees and companies
- Import employees and companies from an excel document
- Authentication


### Frontend

A single page application shall be implemented.

The frontend shall provide al list view of companies with at least the properties: business_name, industry, type.
How to assign employees (first name, surname, email, date_of_birth) to the company and to show already assigned users is up to you.

**Optional**

- Authentication
- Enable to switch between employees and companies in the main list
- Show employees with no assigned company
- Show a selected company and the assigned employees on a map

### DevOps
All code should be commited to a private repository on https://github.com/ with meaningful commit messages. Add the github-user 'tziea' into the repository. The code should be structured as follows.

```bash
├── backend
├── frontend
├── docker-compose.yml
└── README.md # repo documentation and instructions
```

A `docker-compose.yml` file shall be provided, which will automatically build and run all components by calling `docker-compose up`. General documentation of the repo and instructions how to build and run the application shall be provided in the `README.md`.

