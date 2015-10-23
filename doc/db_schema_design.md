# Database Schema
> Descript...

## tms_users
> Descript...

| Field      | Type             | Null | Key |
| ---------- |:----------------:| ----:| ---:| 
| id         | int(10) unsigned | NO   | PRI |
| name       | varchar(100)     | NO   |     |
| gender     | tinyint(2)       | NO   |     |
| avatar_url | varchar(255)     | NO   |     |
| password   | varchar(255)     | NO   |     |
| group_id   | int(10)          | NO   |     |
| created_by | int(10)          | NO   |     |
| created_at | timestamp        | NO   |     |
| updated_at | timestamp        | NO   |     |

 
## tms_user_groups
> Descript...

| Field      | Type             | Null | Key |
| ---------- |:----------------:| ----:| ---:| 
| id         | int(10) unsigned | NO   | PRI |
| name       | varchar(100)     | NO   |     |
| parent_id  | int(10)          | NO   |     |
| created_by | int(10)          | NO   |     |
| created_at | timestamp        | NO   |     |
| updated_at | timestamp        | NO   |     |


## tms_roles
> Descript...

| Field      | Type             | Null | Key |
| ---------- |:----------------:| ----:| ---:| 
| id         | int(10) unsigned | NO   | PRI |
| name       | varchar(100)     | NO   |     |
| created_by | int(10)          | NO   |     |
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
| created_by | int(10)          | NO   |     |
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
| order      |  int(10)         | NO   |     |
| created_by | int(10)          | NO   |     |
| created_at | timestamp        | NO   |     |
| updated_at | timestamp        | NO   |     |

 
