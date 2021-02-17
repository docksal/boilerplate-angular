# Angular boilerplate for Docksal

[Angular](https://angular.io)

The Angular project was generated with [Angular CLI](https://github.com/angular/angular-cli).

## Instructions

Run `fin init` to install Angular's default starter project.
Once the site is installed, Docksal will start Angular in the development mode,
allowing you to jump to playing with the installation. Edit pages under `docroot/src`.

**Note:** `fin init` always re-creates the project from scratch. To just (re)start the project development server use `fin develop`.

## Development server

Run `fin develop` for a dev server. Navigate to your virtual host for your project (e.g., http://angular.docksal). The app will automatically reload if you change any of the source files.
(note: Angular will point to http://localhost:3000/ - don't use that)

## Code scaffolding

Run `fin exec ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `fin exec ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `fin exec ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `fin exec ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `fin exec ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

This project is set up with the "node" stack which does not come with a database service. If you are doing development that requries a local database service, you will
need to add it to your docksal.yml file. 

```
services:
  # DB
  db:
    extends:
      file: ${HOME}/.docksal/stacks/services.yml
      service: mysql
```

