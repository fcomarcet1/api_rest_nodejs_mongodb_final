# api-rest-nodejs-mongodb
# ROUTES 
##AUTH
    -REGISTER: (POST) //localhost:3099/api/auth/register
        -Inputs: [name, surname, email, password]

    -LOGIN: (POST) http://localhost:3099/api/auth/login
        -Inputs: [email, password]
    
    -ACTIVATE ACCOUNT (PATCH) http://localhost:3099/api/auth/activate
        -Inputs: [email, code]

    -RESET CONFIRMATION CODE (PATCH) http://localhost:3099/api/auth/refresh-confirmationCode
         -Inputs: [email]

##USER
    -SHOW: User profile: (GET) http://localhost:3099/api/user/show

    -GET ALL: Users list [ROLE_ADMIN]: (GET) http://localhost:3099/api/user/all

    -EDIT: Fill form edit user (GET) http://localhost:3099/api/user/edit

    -EDIT: Update user account (PUT) http://localhost:3099/api/user/edit
        -Inputs: [name, surname, email]

    

##ADMIN
    -REGISTER: (POST) //localhost:3099/api/auth/register
        -Inputs: [name, surname, email, password]

    -LOGIN: (POST) http://localhost:3099/api/auth/login
        -Inputs: [email, password]

ADMIN[ROLE_ADMIN]:
-Admin profile: (GET)  http://localhost:3099/api/admin/profile
-All users : (GET) http://localhost:3099/api/admin/users
-User detail: (GET)
-Delete user Account: (DELETE)

USER[ROLE_USER]:
-User profile: (GET) http://localhost:3099/api/user/show
-User edit (GET) http://localhost:3099/api/user/edit
-User update profile: (PUT) http://localhost:3099/api/user/update
-User upload avatar (POST) http://localhost:3099/api/upload/avatar
-Get user avatar (GET) http://localhost:3099/api/user/avatar/:fileName
-Delete user Account: (DELETE) http://localhost:3099/api/user/delete
"# api_rest_nodejs_mongodb_final" 
