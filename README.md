# Aurelia GetStarted Client (for framework discovery)

## Aurelia Skeleton

This project base on [aurelia-skeleton-navigation](https://github.com/aurelia/skeleton-navigation/releases), v0.10.
To init the project :
  * `npm install`
  * `npm install -g gulp`
  * `npm install -g jspm`
  * (jspm endpoint config github)
  * `jspm install -y`
  * `gulp watch` ( [http://localhost:9000](http://localhost:9000) )

## Running The Unit Tests

To run the unit tests, first ensure that you have followed the steps above in order to install all dependencies and successfully build the library. Once you have done that, proceed with these additional steps:

### Requirement
  
  * `npm install -g karma-cli`
  * `jspm install aurelia-framework`
  * `jspm install aurelia-http-client`
  * `jspm install aurelia-router`

### Start
  
  `karma start
  
### Running The E2E Tests
Integration tests are performed with [Protractor](http://angular.github.io/protractor/#/).

1. Place your E2E-Tests into the folder ```test/e2e/src```
2. Install the necessary webdriver

  ```shell
  gulp webdriver_update
  ```

3. Configure the path to the webdriver by opening the file ```protractor.conf.js``` and adjusting the ```seleniumServerJar``` property. Typically its only needed to adjust the version number.

4. Run the E2E-Tests

  ```shell
  gulp e2e
  ```
