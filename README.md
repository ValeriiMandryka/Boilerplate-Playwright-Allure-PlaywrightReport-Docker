# Boilerplate-Playwright-PlaywrightReport-AllureReport
Template repository for project based on Playwright framefork with configurated GitHub actions and Allure report. Can be used for auto testing on Chromium/Firefox/Webkit browsers and MobileChrome/MobileSafari also icluded Docker

##  Attantion! To run tests on different browsers Antivirus tool should be switched off 

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

    3.1 npm run Alltests-Headless  - it will run all tast in Hedless mode
    3.2 npm run Alltests-Headed    - it will run all tast in UI mode
    3.3 npm run Tests:Headless-on-Chromium    - it will run all tast in Hedless mode in Chrome browser
    3.4 npm run Tests:Headless-on-Firefox     - it will run all tast in Hedless mode in Firefox browser
    3.5 npm run Tests:Headless-on-Safari      - it will run all tast in Hedless mode in Safari browser
    3.6 npm run Tests:Headless-on-mobileChrome-Pixel5    - it will run all tast in Hedless mode on Mobile Pixel 15
    3.7 npm run Tests:Headless-on-mobileSafari-Iphone12  - it will run all tast in Hedless mode on Mobile Iphone 12
    3.8 npm run Tests:Headed-on-Chromium  - it will run all tast in UI mode in Chrome browser
    3.9 npm run Tests:Headed-on-Firefox   - it will run all tast in UI mode in Firefox browser
    3.10 npm run Tests:Headed-on-Safari   - it will run all tast in UI mode in Safari browser
    3.11 npm run Tests:Headed-on-mobileChrome-Pixel5     - it will run all tast in UI mode on Mobile Pixel 15
    3.12 npm run Tests:Headed-on-mobileSafari-Iphone12   - it will run all tast in UI mode on Mobile Iphone 12
    3.13 npm run open:PlaywriteReport  - it will open Playwright report
    3.14 npm run open:AllureReport     - it will open Allure report

## 4. Running a single test file:
   ```
    npx playwright test landing-page.spec.ts

   ```
   Where landing-page.spec.ts you should to switch the name on your file name 
   
## 4. Run tests in Docker
   # 4.1 Run comand
    
    ```
    npm run StartSelenium-Grid-Server

    ```
   # 4.2 Run comand in Bash terminal
  
   ```
   SELENIUM_REMOTE_URL=http://localhost:4444/wd/hub npx playwright test --config=docker.config.js

   ```
  
