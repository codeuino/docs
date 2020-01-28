# Badge and point allotment Api

Priority:- High

\*\*\*\*

## Summary

In Codebadge, presently all the badge allotment computation are taking place at browser level. We require to shift all the badge related computation at backend using nodejs API. The task to be preformed under this task are:-

* Designing a database schema to manage user points for projects and organization, storing badge templates in efficient manner, storing admin defined pattern for awarding badges and special badges.
* Design a badge allotment api which shall fulfill following criterias:-
  * Admin can decide the count of points for alloting points.
  * Using Machine Learning allocating points as per past relatable issues.
  * Designing a special badge allotment system which can be decided by the admin while creating an account.
* Designing an api system which returns renderable badges. Badges must be saved in minified format which shall be improved in quality and size on rendering time.
* Creating shareable illustrator system which admin can only share with his organization contributors using email/github username.
* Fetching contribution outside browser without using cron jobs approach which makes the computation speed slower.

  **Required Skills/knowledge:**

* Good knowledge of databases
* languages such as NodeJs
* experience of working sockets programming and using github apis
* Good Knowledge of Modules Bundling

#### Difficulty Level: Moderate

#### Mentors

