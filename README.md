# Busy Hours

Busy Hours is web tool to allow easy editing of OpenStreetMap public transport hours.


## Develop

To run the project locally, you need to first `git clone` this repository, and have NodeJS >= 9 installed on your computer.

Then, install project dependencies using `npm install`. Now, you can use following commands to work.

### `npm start`

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.<br>
You will also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.<br>
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.


## Translations

Translations of user interface labels are managed using JSON configuration files, automatically generated using `i18nline` tool. When editing code, launch manually `npm run i18n:build` to update these configuration files.


## Documentation

Documentation of the source code uses [JSDoc syntax](http://usejsdoc.org/). Readable documentation can be generated using `npm run doc` command, and will be available as an HTML page in `doc/` folder.


## Configuration

Various components of the editor can be configured for the instance manager. Main files you can edit are :

* `src/config/config.json` : various configurations, in particular [OAuth tokens](https://wiki.openstreetmap.org/wiki/Oauth) and [OSM API URL](https://wiki.openstreetmap.org/wiki/API_v0.6#URL_.2B_authentication) to use

You can either make temporary changes by editing these files in your `build/` folder, or making changes permanent by editing in `public/` folder (and rebuild using described procedure above). Note that to take into account changes made in `src/` subfolders, you have to rebuild code (using `npm run build`, see above).
