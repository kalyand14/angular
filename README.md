# angular
This will hold the code snippet and issues/problem that i encountered in my jounery

================================================
Jan 8 2022
================================================

**PROBLEM:**

**Today i tried to setup my angular project and when i tried to run the ng serve i got below error**

Error: node_modules/@angular/platform-browser/platform-browser.d.ts:44:22 - error NG6002: Appears in the NgModule.imports of AppModule, but could not be resolved to an NgModule class.

This likely means that the library (@angular/platform-browser) which declares BrowserModule has not been processed correctly by ngcc, or is not compatible with Angular Ivy. Check if a newer version of the library is available, and update if so. Also consider checking with the library's authors to see if the library is expected to be compatible with Ivy.

44 export declare class BrowserModule {
                        ~~~~~~~~~~~~~

**SOLUTION:**

sudo npx ngcc

After this i try to run ng serve the app is up and running

