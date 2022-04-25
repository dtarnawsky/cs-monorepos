
# Getting Started with NX and Ionic
Get started with an empty workspace, replace `my-org` with your organization name:
`npx create-nx-workspace my-org --preset=empty`

Open up the folder in VS Code or in your terminal `cd my-org`

Make sure you are using v13+ by looking at `package.json` packages with `@nrwl`. Upgrade if needed `13.9.3`
If you had v12 then you may need to run `nx format`

For Angular users: Install the NX extension:
`npm install --save-dev @nxtend/ionic-angular @nxtend/capacitor`

For React users: Install the NX extension:
`npm install --save-dev --exact @nxtend/ionic-react @nxtend/capacitor @nrwl/react`

Create a new app in the workspace replacing myApp with your app name:
`nx generate @nxtend/ionic-angular:application myApp`


