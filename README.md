# github-graphql-server
Learning GraphQL with GitHub API and Express.

## Instructions
* Clone repo and make sure Yarn is installed.
* Inside repo, run ```yarn```.
* Run ```npm start``` and go to localhost:8888/graphql

## Examples
In localhost, you can make calls to the GitHub API like this:
``` javascript
{
  gitHubUser(username: "yourUserNameGoesHere") {
    login,
    avatar_url,
    following,
    following_url,
    users_following {
      login,
      avatar_url,
      users_following {
        login,
        avatar_url
      }
    }
  }
}
```
Additional options are available. To look at these, check out the ./data/schema.js file.
