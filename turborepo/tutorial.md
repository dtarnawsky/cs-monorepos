# TurboRepos and Ionic
In an empty folder get started by running:
`npx create-turbo@latest`

Choose `.` for the location and choose `npm` (or your preferred package manager)

This creates 2 apps in the `apps` folder. You can build all the apps with:
`npx turbo run build`

## Create a fresh Ionic app
Create a new Ionic app with:

`cd apps`
`ionic start`

Choose `n`, then your preferred framework, project name and starter app.


## Building
Running `npx turbo run build` will run the `build` script on all projects
Running `npx turbo run build --scope=my-app` will run the `build` script of `my-app` from the `apps` folder


## Notes
Turborepos is designed by Vercel with a focus on build speed so it has both shared caches and a way to specify project dependencies in the pipeline object of turbo.json




