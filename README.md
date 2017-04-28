# <img src="https://github.com/pip-services/pip-services/raw/master/design/Logo.png" alt="Pip.Services Logo" style="max-width:30%"> <br/> Workspace for User Management Pip.Services

This is a workspace for [User Management Pip.Services](https://github.com/pip-services-users) 
implemented in 5 different languages: .NET, Java, Node.js, Go and Python.

The workspace enables build, test, and release across the following projects:

- **pip-services-devenv** - dockerized infrastructure services for development and testing
- **pip-services-email-node** - Email sendins microservice in Node.js
- **pip-clients-email-node** - Client to Email sending microservice in Node.js
- **pip-services-activities-node** - User activities microservice in Node.js
- **pip-clients-activities-node** - Client to User activities microservice in Node.js
- **pip-services-users-node** - User account microservice in Node.js
- **pip-clients-users-node** - Client to User account microservice in Node.js
- **pip-services-passwords-node** - Password authentication microservice in Node.js
- **pip-clients-passwords-node** - Client to Password authentication microservice in Node.js
- **pip-services-roles-node** - Role authorization microservice in Node.js
- **pip-clients-roles-node** - Client to Role authorization microservice in Node.js
- **pip-services-sessions-node** - Session management microservice in Node.js
- **pip-clients-sessions-node** - Client to Session management microservice in Node.js
- **pip-services-settings-node** - User settings microservice in Node.js
- **pip-clients-settings-node** - Client to User settings microservice in Node.js
- **pip-facade-users-node** - Facade operations for user management microservices in Node.js

## Installation

- Install **pip-tasks-ps**, **pip-tasks-common-ps** and **pip-tasks-node-ps** Powershell modules, 
add them to **PSModulePath** and import into Powershell

- Clone this workspace to local disk
```bash
> git clone https://github.com/pip-services-users/pip-services-users-ws.git
```

- Got to the workspace folder and clone component repositories
```bash
> piptask clone -workspace
```

## Usage

- Setting default workspace
```bash
> pipuse <Path to this workspace>
```

- Start and stop infrastructure services
```bash
> piptask start -component pip-services-devenv
> piptask stop -component pip-services-devenv
```

- Building all components
```bash
> piptask build -all
```

- Test all components
``` bash
> piptask test -all
```

- Check out changes from remote repository
```bash
> piptask pull -all
```

- Check in changes to remote repository
```bash
> piptask push -m <Changes comment> -all
```

## Acknowledgements

The User Management Pip.Services are created and maintained by **Sergey Seroukhov**
