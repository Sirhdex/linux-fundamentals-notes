## Concepts
- Admin responsibilites often include creation of new users + assigning specific users to groups (maintaining security)
- sudo commands allow for privileged users to execute actions otherwise only permitted by user
- Effective user management allows for proficient vulnerability identifiction and exploit misconfiguration


## Commands
- su -- request user permissions and switches to that user id
- useradd -- creates new user
- userdel -- deletes new user
- usermod -- modifies new user
- addgroup -- adds group to the system
- delgroup -- deletes group from the system
- passwd -- changes password

## Examples
- /etc/passwd - encrypted password cache for all users 

## Answers
- useradd -m
- usermod --lock
- su --command