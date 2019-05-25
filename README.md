# [Work in progress]

## About the project

Luftcms is a scaffolding project, ***this is not a framework this is just a project kickstarter kit for your small/mid sized projects***

Goals of this scaffolding is to:
1. Speed up development of small/mid sized projects by preparing common design/setup and code base.
2. Have an identical "real hello world" project in multiple languages/frameworks/tech-stacks, identical requirements, and design, for comparison purpose and mainly as a teaching/self-learning material.
3. (Better goal? Send your suggestion!)

## Requirements

The project should be deployable as one of the following
- <u><b>Setup A</b></u>: Backend API + 2 frontend apps  (dashboad & client)
- <u><b>Setup B</b></u>: Backend as a Service(eg: firebase) + Frontend Admin panel + frontend client app
- <u><b>Setup C</b></u> (Not confirmed): Classic Server side template app (document based application)

### Main features (Setup A)

- API should match the Open API Specifications file: [openapi.yaml](https://luftcms.com/openapi.yaml)
- **OAUTH2** Authentication (At this stage we'll use oauth2 Password based grant only)
- **Payment gateway**
    - Paypal
    - Skrill
- User roles starting by default with three roles
    - Admin
    - Supervisor (Read/Write)
    - Client (Normal user Read + Read/Write owned items)
- **Item:** The main model in the project and depending on the project this is the (Article in a blog, Product in a simple ecommerce store, store in a stores directory app... and so on)
- **Item Type:** Classification of items by the app not the user. (Example: Article or product)
- **Item meta:** Extend item properties
- **Item actions:** Actions user can take on an item and permission required for that action (Actions like: comment, buy, review, thumbs up)
- **Tags:** Tags are shared across the system unlike collection which is personalized for users.
- **Item collections:** User should be able to create a list/collection of items, for example favorite movies list, favorite stores, if this is used in a simple ecommerce a shopping card.


## Parts, Languages & Frameworks

| Setup | Part      | Language/Framework          | State      | Repo                                                                              | 
|-------|-----------|------------------------------|------------|-----------------------------------------------------------------------------------|
| A     | API       | PHP/Laravel                  | WIP        | [luftcms-api-laravel](https://github.com/luftcms/luftcms-api-laravel)            |
| A     | Dashboard | JS/React                     | WIP        | [luftcms-dashboard-react](https://github.com/luftcms/luftcms-dashboard-react)    | 
| A     | Client    | JS/React                     | WIP        | [luftcms-client-react](https://github.com/luftcms/luftcms-client-react)          | 
| A     | Dashboard | JS/EmberJs                   | Planned    | N/A
| A     | Client    | JS/EmberJs                   | Planned    | N/A
| A     | Dashboard | JS/Angular                   | TBD        | N/A                                                                               | 
| A     | Client    | JS/Angular                   | TBD        | N/A                                                                               | 
| A     | Client    | JS/React-Native              | Planned    | N/A                                                                               |
| A     | API       | PHP/vanilla                  | Planned    | N/A                                                                               |
| A     | API       | PHP/symfony                  | Planned    | N/A                                                                               |
| A     | API       | Python/Django or Flask       | TBD        | N/A                                                                               | 
| A     | API       | golang                       | TBD        | N/A                                                                               | 
| B     | Dashboard | JS/React+firebase            | WIP        | N/A                                                                               | 
| B     | Client    | JS/React+firebase            | WIP        | N/A                                                                               | 


## Roadmap:

As an immature open-source project the roadmap is not defined with timeline, but milestones/todos so this is just the big picture:
1. Finish a Well defined feasable requirements (Including models structure, expected API endpoints).
2. Develop the API first [luftcms-api-laravel](https://github.com/luftcms/luftcms-api-laravel)
3. MVP frontend apps (dashboard & client app).
4. Refining iterations and redefine requirement if needed.
5. Mobile app 
6. Start with other 'Planned' and 'To Be Discussed' languages & frameworks.

## Contributions:

**Contributions wanted!** 

If you can to contribute in a specific part of the project directly create an issue/PR in that part repo, if you want to suggest modifications to the whole project requirements or sepecifications or want to add a new part/language/framework create an issue/PR in the main repo with your suggestion.<br />

Specifications/Requirements are flexible at this point, once the project grows changing the specifications/requirements will be a little more strict but this will be decided by the community later<br />

This project is a WIP, please don't use the scaffolding before a stable release is ready.<br />
