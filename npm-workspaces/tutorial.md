# NPM Workspaces
Workspace folder is set in the root `package.json` with:
```
"workspaces": [
    "apps/*"
  ]
```

Running `npm install` will install all dependencies from each of the apps

If you have an workspace with a name `my-app1` you can run the `build` script of it with:
`npm run build --workspace=my-app1`

or serve it with:
`npm run start --workspace=my-app1`

`npm list --workspace=my-app1`

`npx ionic build --project=my-app2`

You can `cd` to the folder and run `cap` commands

### Ionic quirk
Ionic cli handles multi-repo using `ionic.config.json`, if a project name is `my-app1` and the project is Angular then `angular.json` needs to have a project with name `my-app1` - it cannot be `app` which is the default.

## React quirk
Running `npx ionic build --project=my-app2` from the root could error with:
`Failed to load config "react-app" to extend from.`
To fix it required `npm install` be run from the workspace `my-app2`

## React quirk 2
Starter for react creates a config with `www` as the `webDir` however React will create a `build` folder. Bug??