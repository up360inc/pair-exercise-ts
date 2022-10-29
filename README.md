## Pair Programming Exercise

### Tasks

1. enter a github username and fetch a list of the user's public repositories
2. display them in a list
3. show a total count
4. provide a link to the repo on github
5. allow sorting by name
6. allow filtering by topic
7. allow filtering by language

### Github API references

#### List user repositories

https://docs.github.com/en/rest/repos/repos#list-repositories-for-a-user

```js
// Octokit.js
// https://github.com/octokit/core.js#readme
const octokit = new Octokit({
  auth: "YOUR-TOKEN",
});

await octokit.request("GET /users/{username}/repos", {
  username: "USERNAME",
});
```
