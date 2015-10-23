# Database Schema
> Descript...

## tms_users
> Descript...

| Field      | Type             | Null | Key |
| ---------- |:----------------:| ----:| ---:| 
| id         | int(10) unsigned | NO   | PRI |
| name       | varchar(100)     | NO   |     |
| gender     | tinyint(2)       | NO   |     |
| is_admin   | tinyint(2)       | NO   |     |
| avatar_url | varchar(255)     | NO   |     |
| password   | varchar(255)     | NO   |     |
| created_at | timestamp        | NO   |     |
| updated_at | timestamp        | NO   |     |



## tms_roles
> Descript...

| Field      | Type             | Null | Key |
| ---------- |:----------------:| ----:| ---:| 
| id         | int(10) unsigned | NO   | PRI |
| name       | varchar(100)     | NO   |     |
| created_at | timestamp        | NO   |     |
| updated_at | timestamp        | NO   |     |


## tms_menus
> Descript...

| Field      | Type             | Null | Key |
| ---------- |:----------------:| ----:| ---:| 
| id         | int(10) unsigned | NO   | PRI |
| name       | varchar(100)     | NO   |     |
| parent_id  | int(10)          | NO   |     |
| link_url   | varchar(255)     | NO   |     |
| is_folder  | tinyint(2)       | NO   |     |
| icon_url   | varchar(255)     | NO   |     |
| order      |  int(10)         | NO   |     |
| created_at | timestamp        | NO   |     |
| updated_at | timestamp        | NO   |     |


## tms_permissions
> Descript...

| Field      | Type             | Null | Key |
| ---------- |:----------------:| ----:| ---:| 
| id         | int(10) unsigned | NO   | PRI |
| name       | varchar(100)     | NO   |     |
| parent_id  | int(10)          | NO   |     |
| actions    | varchar(255)     | NO   |     |
| desc       | varchar(255)     | NO   |     |
| created_at | timestamp        | NO   |     |
| updated_at | timestamp        | NO   |     |


## tms_user_role
> Descript...

| Field      | Type             | Null | Key |
| ---------- |:----------------:| ----:| ---:| 
| id         | int(10) unsigned | NO   | PRI |
| user_id    | int(10)          | NO   |     |
| role_id    | int(10)          | NO   |     |
| created_at | timestamp        | NO   |     |
| updated_at | timestamp        | NO   |     |



## tms_role_menu
> Descript...

| Field      | Type             | Null | Key |
| ---------- |:----------------:| ----:| ---:| 
| id         | int(10) unsigned | NO   | PRI |
| role_id    | int(10)          | NO   |     |
| menu_id    | int(10)          | NO   |     |
| created_by | int(10)          | NO   |     |
| created_at | timestamp        | NO   |     |
| updated_at | timestamp        | NO   |     |


## tms_role_permission
> Descript...

| Field        | Type             | Null | Key |
| ----------   |:----------------:| ----:| ---:| 
| id           | int(10) unsigned | NO   | PRI |
| permission_id| int(10)          | NO   |     |
| role_id      | int(10)          | NO   |     |
| created_at   | timestamp        | NO   |     |
| updated_at   | timestamp        | NO   |     |

