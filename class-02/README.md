# Class 02 - Basic concepts of Angular

The second class was given the 08/03/18 via Webex.
On this, the teacher provides the basic concepts of Angular.

## Index
- Architecture
- Angular Modules
- Angular Components
- Data Binding

## Architecture
When you create an App from Scratch, you found the following files or folders:
- `e2e` End to end testing or also known as integration testing is a great way to make sure at a high-level overview that our applications function correctly
- `node_modules` When you work with npm locally, this tool drop your packages in that directory
- `angular-cli.json` It's storage settings of Angular CLI
- `karma.conf.js` This contains all the configurations for your tests
- `package.json` This file lists the packages that your project depends on
- `protractor.conf.js` Protractor is an end-to-end test framework for Angular applications. Here we can set all the configurations for that tool
- `tsconfig.json` File that specifies the root files and the compiler options required to compile the project
- `tslint.js` File that specifies the config for the linter.
- `app` That folder contains all the components and artifacts of your App
- `assets` Here you can found all the static files, like images, sprites, documents.
- `environments` This folder contains all the settings and environment variables
- `main.ts` It's the entry point of your application, compiles the application with just-in-time and bootstraps the application

## Angular Modules
Applications on Angular are modular. @NgModule is the system of modularity that this implement.

Each module on Angular is a class with the @NgModule decorator.

These are some examples:
- FormsModule, HttpClientModule, and RouterModule are modules of Angular
- Material Design, Ionic are modules of thirds

## Angular Components
`@Component` decorator define that class how to an Angular component and allow proportionate some of the following metadata:

- selector
- providers
- template
- templateUrl
- styles
- stylesUrls
- animations

## Data Binding
This concept explains how the data are sync between the model of the component and the view.

Types of data binding:
- Interpolation
- Property Binding
- Event Binding
- Two-Way Binding