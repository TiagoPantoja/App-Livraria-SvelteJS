# App-Livraria-SvelteJS

Looking for a shareable component template? Go here --> sveltejs/component-template

svelte app
This is a project template for Svelte apps. It lives at https://github.com/sveltejs/template.

Create a new project based on this template using degit:

npx degit sveltejs/template svelte-app
cd svelte-app
Note that you will need to have Node.js installed.

Get started
Install the dependencies

cd svelte-app
npm install
then start Rollup:

npm run dev
Navigate to localhost:5000. You should see your app running. Edit a component file in src, save it, and reload the page to see your changes.

By default, the server will only respond to requests from localhost. To allow connections from other computers, edit the sirv commands in package.json to include the option --host 0.0.0.0.

Building and running in production mode
Create an optimised version of the app:

npm run build
You can run the newly built app with npm run start. This uses sirv, which is included in your package.json's dependencies so that the app will work when you deploy to platforms like Heroku.

Single-page app mode
By default, sirv will only respond to requests that match files in public. This is to maximise compatibility with static fileservers, allowing you to deploy your app anywhere.

If you're building a single-page app (SPA) with multiple routes, sirv needs to be able to respond to requests for any path. You can make it so by editing the "start" command in package.json:

"start": "sirv public --single"
Deploying to the web
With now
Install now if you haven't already:

npm install -g now
Within your project folder:

cd public
now deploy --name my-project
As an alternative, use the Now desktop client and simply drag the unzipped project folder to the taskbar icon.

With surge
Install surge if you haven't already:

npm install -g surge
From within project folder:

npm run build
surge public my-project.surge.sh
