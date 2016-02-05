# Challenge GitHub API

## Goal
This challenge is aim to learn "How to access GitHub API through Node.js".

## Requirements
- Node.js ([https://nodejs.org/](https://nodejs.org/))
- GitHub Token: ([https://github.com/settings/tokens](https://github.com/settings/tokens))
- Local submission is recommended

### Set local environment

If you take this challenge from your local environment, you need to set github personal token as environment variable with name `GITHUB_TOKEN`.

If you are not familiar with setting local environment, you can set environment through file named `specifications/env.json`. Inside file, set `GITHUB_TOKEN` as a key name and your token as a value.  
File should be like below.

```json
{
  "GITHUB_TOKEN": "github personal token that you can get"
}
```

## Steps
### Get user information
GitHub provides an endpoint to get a user information.
Write a program to get user information based on passed user name.

For more details of how to get a single user, please look through [this API document](https://developer.github.com/v3/users/#get-a-single-user).

### Get user repositories
You can access to public repositories of all users. Implement a function to get repository information from specified user.
Also, accept parameters to set options for listing API.

For more details of how to get list of user repositories, please look through [this API document](https://developer.github.com/v3/repos/#list-user-repositories).

### Create and Edit Issues
User can create issues on any public repositories. Also, editing issues are possible if you are the creator of issues or you have permission to edit by such as collaborator settings.
Implement two functions; function to create an issue and edit an issue.

To know about endpoints related to issues, please look through [this API document](https://developer.github.com/v3/issues/#create-an-issue).
