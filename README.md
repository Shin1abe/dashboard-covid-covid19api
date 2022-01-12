This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app), using the [Redux](https://redux.js.org/) and [Redux Toolkit](https://redux-toolkit.js.org/) template.

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.<br />
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br />
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br />
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br />
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br />
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
============= firebase hosting =============
https://console.firebase.google.com/project/dashboard-covid-covid19api/overview?hl=ja
------------update deploy method-------------------------------
npm run build
(firebase login)
firebase deploy
------------initial setup method-------------------------------
npm run build
npm install -g firebase-tools
firebase login
firebase init
firebase deploy
------------initial setup history-------------------------------
PS C:\MyPrj\playground\dashboard-covid-covid19api> firebase init

     ######## #### ########  ######## ########     ###     ######  ########
     ##        ##  ##     ## ##       ##     ##  ##   ##  ##       ##
     ######    ##  ########  ######   ########  #########  ######  ######
     ##        ##  ##    ##  ##       ##     ## ##     ##       ## ##
     ##       #### ##     ## ######## ########  ##     ##  ######  ########

You're about to initialize a Firebase project in this directory:

C:\MyPrj\playground\dashboard-covid-covid19api

Before we get started, keep in mind:

- You are currently outside your home directory

? Are you ready to proceed? Yes
? Which Firebase features do you want to set up for this directory? Press Space to select features, then Enter to confirm your choices. Hosting: Configure files
for Firebase Hosting and (optionally) set up GitHub Action deploys

=== Project Setup

First, let's associate this project directory with a Firebase project.
You can create multiple project aliases by running firebase use --add,
but for now we'll just set up a default project.

? Please select an option: Use an existing project
? Select a default Firebase project for this directory: dashboard-covid-covid19api (dashboard-covid-covid19api)
i Using project dashboard-covid-covid19api (dashboard-covid-covid19api)

=== Hosting Setup

Your public directory is the folder (relative to your project directory) that
will contain Hosting assets to be uploaded with firebase deploy. If you
have a build process for your assets, use your build's output directory.

? What do you want to use as your public directory? build
? Configure as a single-page app (rewrite all urls to /index.html)? No
? Set up automatic builds and deploys with GitHub? Yes

- Wrote build/404.html
  ? File build/index.html already exists. Overwrite? No
  i Skipping write of build/index.html

i Detected a .git folder at C:\MyPrj\playground\dashboard-covid-covid19api
i Authorizing with GitHub to upload your service account to a GitHub repository's secrets store.

Visit this URL on this device to log in:
https://github.com/login/oauth/authorize?client_id=89cf50f02ac6aaed3484&state=529081145&redirect_uri=http%3A%2F%2Flocalhost%3A9005&scope=read%3Auser%20repo%20public_repo

Waiting for authentication...

- Success! Logged into GitHub as Shin1abe
  https://github.com/login/oauth/authorize?client_id=89cf50f02ac6aaed3484&state=529081145&redirect_uri=http%3A%2F%2Flocalhost%3A9005&scope=read%3Auser%20repo%20public_repo

Waiting for authentication...

- Success! Logged into GitHub as Shin1abe

? For which GitHub repository would you like to set up a GitHub workflow? (format: user/repository) Shin1abe/dashboard-covid-covid19api

- Created service account github-action-447010953 with Firebase Hosting admin permissions.
- Uploaded service account JSON to GitHub as secret FIREBASE_SERVICE_ACCOUNT_DASHBOARD_COVID_COVID19API.
  i You can manage your secrets at https://github.com/Shin1abe/dashboard-covid-covid19api/settings/secrets.

? Set up the workflow to run a build script before every deploy? Yes
? What script should be run before every deploy? (npm ci && npm run build) npm ci && npm run build
? What script should be run before every deploy? npm ci && npm run build

- Created workflow file C:\MyPrj\playground\dashboard-covid-covid19api\.github/workflows/firebase-hosting-pull-request.yml
  ? Set up automatic deployment to your site's live channel when a PR is merged? Yes
  ? What is the name of the GitHub branch associated with your site's live channel? main

- Created workflow file C:\MyPrj\playground\dashboard-covid-covid19api\.github/workflows/firebase-hosting-merge.yml

i Action required: Visit this URL to revoke authorization for the Firebase CLI GitHub OAuth App:
https://github.com/settings/connections/applications/89cf50f02ac6aaed3484
i Action required: Push any new workflow file(s) to your repo

i Writing configuration info to firebase.json...
i Writing project information to .firebaserc...

- Firebase initialization complete!
  PS C:\MyPrj\playground\dashboard-covid-covid19api> firebase deploy

=== Deploying to 'dashboard-covid-covid19api'...

i deploying hosting
i hosting[dashboard-covid-covid19api]: beginning deploy...
i hosting[dashboard-covid-covid19api]: found 19 files in build

- hosting[dashboard-covid-covid19api]: file upload complete
  i hosting[dashboard-covid-covid19api]: finalizing version...
- hosting[dashboard-covid-covid19api]: version finalized
  i hosting[dashboard-covid-covid19api]: releasing new version...
- hosting[dashboard-covid-covid19api]: release complete

- Deploy complete!

Project Console: https://console.firebase.google.com/project/dashboard-covid-covid19api/overview
Hosting URL: https://dashboard-covid-covid19api.web.app
PS C:\MyPrj\playground\dashboard-covid-covid19api>
