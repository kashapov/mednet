This project was bootstrapped with [Create React App](https://github.com/facebookincubator/create-react-app).
Please, see `Docs/README_boot.md` for lots of information.

Here you will find ADDITIONAL information, specific to the project.

# Deployment
`npm run build` creates Production build.
To run it locally on `http://localhost:5000` do:
```
npm i -g serve
serve -s build
```

# Testing
To run a single test, do:
```
npm test -- -t "Sidebar.test.js"
npm run test --watch --findRelatedTests src/containers/App/tests/reducer.test.js
```

Run tests related to changed files based on hg/git (uncommitted files):
```
npm run test -- -o
```

# API endpoints

LogIn
```
// method: POST

http://www.teamcofounder.com/api/v1/mednet/login

// body
{ email: demo@demo.com, password: demo }

// response is something like this
{
  "profile": {
    "dateOfBirth":"1986-04-12T00:00:00.000Z",
    "lastName":"Smith",
    "firstName":"John",
  },
  "position":"manager",
  "permissions": ["statistics"],
  "employee":true
}
```

LogOut
```
// method: POST

http://www.teamcofounder.com/api/v1/mednet/logout
```

Get banner products
```
// method: GET

http://www.teamcofounder.com/api/v1/mednet/bannerProducts
```
