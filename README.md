# Angular Drone Sonar

[![Build Status](https://drone.jmerle.dev/api/badges/jmerle/angular-drone-sonar/status.svg)](https://drone.jmerle.dev/jmerle/angular-drone-sonar)
[![Quality Gate Status](https://sonar.jmerle.dev/api/project_badges/measure?project=jmerle%3Aangular-drone-sonar&metric=alert_status)](https://sonar.jmerle.dev/dashboard?id=jmerle%3Aangular-drone-sonar)
[![Coverage](https://sonar.jmerle.dev/api/project_badges/measure?project=jmerle%3Aangular-drone-sonar&metric=coverage)](https://sonar.jmerle.dev/dashboard?id=jmerle%3Aangular-drone-sonar)
[![Maintainability Rating](https://sonar.jmerle.dev/api/project_badges/measure?project=jmerle%3Aangular-drone-sonar&metric=sqale_rating)](https://sonar.jmerle.dev/dashboard?id=jmerle%3Aangular-drone-sonar)
[![Security Rating](https://sonar.jmerle.dev/api/project_badges/measure?project=jmerle%3Aangular-drone-sonar&metric=security_rating)](https://sonar.jmerle.dev/dashboard?id=jmerle%3Aangular-drone-sonar)

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.3.8.

This is just a little playground to get Angular working with Drone CI as build server and SonarQube for static code analysis with code coverage reporting.

## Changes

Here are the changes that were made to the standard angular-cli project:
- Prettier has been added with some additional tools: `npm i -D husky lint-staged prettier tslint-config-prettier prettier-check`
- The `package.json` file has been updated with new `lint`, `lint:fix` and `prettier` commands, and with `husky`, `lint-staged` and `prettier` configuration
- The `tslint.json` file has been updated to extend `tslint-config-prettier`
- The `.drone.yml` file has been added with the Drone CI pipeline configuration
- The `src/karma.conf.js` and the `e2e/protractor.conf.js` files have been updated to make tests run successfully in a Docker container
- The `sonar_token` secret has been added to the Drone CI configuration with a SonarQube token that has permission to execute analyses
- The `README.md` file has been updated with Drone CI and SonarQube badges

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
