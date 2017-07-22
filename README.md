# myBootstrap3

## Custom Bootstrap made Easy™
---


### Link to this module
```
# in the myBootstrap3 directory
$ npm link
# back to project root folder
$ cd ../path-to-project
$ npm link myBootstrap3
```

### Import myBootstrap3 in new project
```
# previously
# import 'bootstrap-sass/dist/css/bootstrap.css'
# using this package:
import 'myBootstrap3'
```

### Rebuild project after change to myBootstrap
```
# In project package.json
"scripts": {
    "start-js": "react-scripts start",
    "start": "npm-run-all -p start-js start:myBootstrap3",
    "start:myBootstrap3": "(cd node_modules/myBootstrap3 && npm start)",
    ...
```