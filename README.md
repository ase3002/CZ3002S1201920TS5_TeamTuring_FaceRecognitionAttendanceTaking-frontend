# Frontend - Face-recognition Based Attendance Taking System 

## Setup
First, make sure you have `node v11.10.1` and `npm v6.7.0` installed.

Run the following bash commands to set up the project:
```sh
# clone the project
git clone https://github.com/QiuHaohao/facial-attendance-frontend.git
cd facial-attendance-frontend
# install packages
npm install
```

To start the development server:

```sh
npm start
```

Once the server is started, the client Web App will be accessible at `http://localhost:3000`.

### Configuring Server
By default, the URL of the backend server is `172.21.148.166:8000`, our school server, which can only be accessed in university network. It can be configured by changing `urlBase` attribute of `src/api/config.json`. For example, to connect to the backend server running at `localhost:8000`, change `urlBase` attribute of `src/api/config.json` as follows:

```
{
  "urlBase": "http://localhost:8000",
  ...
}
```

## Deployment
Run 
```sh
npm run deploy
``` 
to build the project locally and upload the static files built to the virtual server `VMadmin@172.21.148.166`.

If you just want to upload the static files built, run
```sh
npm run serve
```

## Available Scripts

In the project directory, you can run:

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

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (Webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

