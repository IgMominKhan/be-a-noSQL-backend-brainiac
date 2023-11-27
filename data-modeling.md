<h1 style="text-align: center;">Data Modeling for PH University</h1>

### User

- \_id
- Id (generated)
- Password
- NeedsPasswordChange
- Role
- Is Deleted
- Created At
- Updated At

### Student

- \_id -Id (Student Id)
- Designation
- Name
- Role
- Gender
- Date of birth
- email
- Contact Number
- Emergency Contact Number
- Present Address
- Permanent Address
- Guardian
- Local Guardian
- Profile Image
- Status
- Academic Department
- Is Deleted
- Created At
- Updated At

### Teacher

- \_id
- Id (Teacher Id)
- Designation
- Name
- Gender
- Date of birth
- email
- Contact Number
- Emergency Contact Number
- Present Address
- Permanent Address
- Profile Image
- Status
- Academic Department
- Academic Teacher
- Is Deleted
- Created At
- Updated At

### Admin

- \_id
- Id (Teacher Id)
- Designation
- Name
- Gender
- Date of birth
- email
- Contact Number
- Emergency Contact Number
- Present Address
- Permanent Address
- Profile Image
- Status
- Academic management
- Is Deleted
- Created At
- Updated At

## ER Diagram
[ph-university ER Diagram](https://lucid.app/lucidchart/8b7e88f6-f279-43d8-a906-877679e64116/edit?view_items=VA9Q73CZiMHB&invitationId=inv_2468a2be-d750-42f9-bb70-76ab710ed613) 

<h1 style="text-align: center;">API Endpoints</h1>

- **users**

  - users/create-student - **POST** - create student
  - users/create-teacher - **POST** - create teacher
  - users/create-admin - **POST** - create admin

- **students**

  - students - **POST** - get all student
  - students/:id - **GET** - get a student
  - students/:id - **PATCH** - update a student
  - students/:id- **DELETE** - delete a student
  - students/my-profile - **GET** - view profile of student

- **teachers**
  - teachers - **POST** - get all teacher
  - teachers/:id - **GET** - get a teacher
  - teachers/:id - **PATCH** - update a teacher
  - teachers/:id- **DELETE** - delete a teacher
  - teachers/my-profile - **GET** - view profile of teacher
  
- **admins**
  - admins - **POST** - get all admin
  - admins/:id - **GET** - get a admin
  - admins/:id - **PATCH** - update a admin
  - admins/:id- **DELETE** - delete a admin
  - admins/my-profile - **GET** - view profile of admin

- **auth**
  - auth/login - **POST** - login
  - auth/logout - **POST** - logout
  - auth/refresh-token - **POST** - refresh
  - auth/forgot-password - **POST** - forgot password
  - auth/reset-password - **POST** - reset password
