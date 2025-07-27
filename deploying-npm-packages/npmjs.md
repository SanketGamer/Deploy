```bash
The Problem is when u create a project in 2 folder(client,server).when u add more functionlaties the codebass will be messy.so can we do a sepperate folder and do the logic there and deploy that folder in an npmpackage and run this packages frontend and backend.
this called your own npm package
1.Go to npmjs.com login
2.go to that folder in vs code and in package.json asign your username like(@sanket1348/common)
3.run this-> npm publish --access=public
4.in your package only dist folder can show-> code .npmignore dist
5.in that common folder in ts.config allow ->declaration:true
6.import the package in backend and frontend it will more cleaner.
```
