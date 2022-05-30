### Gluay Note

- npm start
- npm init
- npm i apollo-server graphql
- npm i nodemon
- package.json "start" : "nodemon index.js"
- npm i lodash

```
const _ = require("lodash");
```

- Apollo GraphQL extention installed

- typeDefs, resolvers

- String, ID, Int, Float, Boolean

- What is enum?

- Sandbox

```
query GetUser($userId: ID!){
  user(id: $userId) {
    name
    age
    nationality
    friends {
      name
    }
  }
}
```

```
{
  "userId": 1
}
```

```
User: {
    favoriteMovies: () => {
      return _.filter(
        MovieList,
        (movie) =>
          movie.yearOfPublication >= 2000 && movie.yearOfPublication <= 2010
      );
    },
  },
```
