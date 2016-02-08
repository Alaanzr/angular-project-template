# Overview

A customised template for creating fully tested Angular applications, based on the angular-seed project. Generic instructions for setting up are below.


## Getting Started (for Mac)
Close the repository using git (downloadable at http://git-scm.com/):

```git clone <insert Github repo link here> ```

### Installing dependencies

The node package manager (npm) houses the back-end dependencies for this project, and a script has been preconfigured to install  front-end dependencies off the back of npm.

To get started therefore, simply type:
```npm install```

You should subsequently find the node_modules and app/bower_components folders in the project directory.


### Running the application
The project utilises the npm's http-server. To start the development web server, type the following:
```npm start```

You can then browse to the application's index page at ```http://localhost:8000/app/index.html```

## Testing

### Running Unit tests

The unit tests for this project have been written in Jasmine and run on the Karma test runner. To run these tests using another preconfigured script, type:

```npm test```

NOTE: All scripts can be found in the package.json file within the project directory.

Karma will continue to run using the above method, so you may wish to carry out a single run of the tests and exit the test runner. To execute a single run:

```npm run test-single-run```

### Running end to end tests

End-to-end tests have also been written in Jasmine and utilise the Protractor test runner. Protractor simulates interaction with the app and verifies that it is responding correctly. Therefore, the web server needs to be serving up the application in order for Protractor to interact with it.

Prior to running end-to-end tests therefore, load up the application server:

```npm start```

Protractor is built upon WebDriver and therefore is dependent on its installation. Please ensure that the stand-alone WebDriver tool is downloaded using the below preconfigured script:

```npm run update-webdriver```

Once the above steps have been carried out, type the below to run the end-to-end tests:

```npm run protractor```

The script will execute the tests against the application being hosted on the development server. As the testing simulates interaction with the application, you may experience minor delays
