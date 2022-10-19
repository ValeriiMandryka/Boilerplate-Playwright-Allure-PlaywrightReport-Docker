# Boilerplate-Playwright-PlaywrightReport-AllureReport
Template repository for project based on Playwright framefork with configurated GitHub actions and Allure report. Can be used for auto testing on Chromium/Firefox/Webkit browsers and MobileChrome/MobileSafari also icluded Docker

 ##                                 NOTICE! To run tests on different browsers Antivirus tool should be switched off 

## Steps to install project

## 1. Run command in VSC:

```
git clone https://github.com/ValeriiMandryka/Boilerplate-Playwright-PlaywrightReport.git

```
## 2. Into root of Project run commands:
```
npm install

npx playwright install

```
## 3. Run tests commands:

   3.1   - it will run all tast in Hedless mode
      
    npm run Alltests-Headles 
   3.2 - it will run all tast in UI mode
    
    npm run Alltests-Headed   
   3.3   - it will run all tast in Hedless mode in Chrome browser
    
    npm run Tests:Headless-on-Chromium
    
       
   3.4   - it will run all tast in Hedless mode in Firefox browser
   
    npm run Tests:Headless-on-Firefox 
   3.5 - it will run all tast in Hedless mode in Safari browser
   
    npm run Tests:Headless-on-Safari      
   3.6- it will run all tast in Hedless mode on Mobile Pixel 15
   
    npm run Tests:Headless-on-mobileChrome-Pixel5    
   3.7 - it will run all tast in Hedless mode on Mobile Iphone 12
   
    npm run Tests:Headless-on-mobileSafari-Iphone12  
   3.8 - it will run all tast in UI mode in Chrome browser
    
    npm run Tests:Headed-on-Chromium  
   3.9 - it will run all tast in UI mode in Firefox browser
   
    npm run Tests:Headed-on-Firefox  
   3.10 - it will run all tast in UI mode in Safari browser
   
    npm run Tests:Headed-on-Safari  
   3.11 - it will run all tast in UI mode on Mobile Pixel 15
      
    npm run Tests:Headed-on-mobileChrome-Pixel5    
   3.12 - it will run all tast in UI mode on Mobile Iphone 12
   
    npm run Tests:Headed-on-mobileSafari-Iphone12   
   3.13- it will open Playwright report
       
    npm run open:PlaywriteReport  
   3.14 - it will open Allure report
   
     npm run open:AllureReport    

## 4. Running a single test file:
   ```
    npx playwright test landing-page.spec.ts

   ```
   Where landing-page.spec.ts you should to switch the name on your file name 
   
## 4. Run tests in Docker
   ### 4.1 Run comand
    
    ```
    npm run StartSelenium-Grid-Server

    ```
   ### 4.2 Run comand in Bash terminal
  
   ```
   SELENIUM_REMOTE_URL=http://localhost:4444/wd/hub npx playwright test --config=docker.config.js

   ```
  ## 5. To run Code Generator :
    
    ```
     npx playwright codegen playwright.dev

   ```
