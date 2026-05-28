# TODO - CodeAlpha_ProjectManagementTool

- [x] Wire React routing: update `client/src/App.jsx` to render `AppRoutes`.

- [x] Add auth client utilities:
  - [x] Create JWT storage helper
  - [x] Create axios instance with Authorization header
  - [x] Create `AuthContext` (login/logout/me)

- [x] Update pages to use backend APIs:
  - [x] Implement Login API call in `client/src/pages/Login/Login.jsx`

  - [x] Implement Register API call in `client/src/pages/Register/Register.jsx`

  - [ ] Make `/dashboard` fetch summary + show real stats in `client/src/pages/Dashboard/Dashboard.jsx`

  - [ ] Make `/projects` fetch projects in `client/src/pages/Projects/Projects.jsx`
  - [ ] Make `/tasks` fetch tasks and render them in `client/src/pages/Tasks/Tasks.jsx`

- [x] Add protected-route wrapper component.

- [x] Real-time updates:
  - [x] Initialize socket.io client on app load after auth
  - [ ] Listen for `task:created`, `task:updated`, `task:deleted`, `notification:*`

  - [ ] Trigger refetch/update on events

- [ ] Run frontend/backend dev servers and do smoke tests.
