# My Angular Journey
This will hold the code snippet and issues/problem that i encountered in my jounery


## Angular usecases

1. Create a portal to show different content based roles -  admin, moderator, user. <br>

   Authentication and authorization <br>
      Github:  https://github.com/bezkoder/angular-12-jwt-refresh-token <br>
      Blogspot: - https://www.bezkoder.com/angular-12-jwt-auth/

## Angular Study videos

1. CURD series - https://www.youtube.com/watch?v=-Zm6lbax308&list=PLVz2XdJiJQxwAhzEZSpDqXlfT7XvNPDIE&index=19
2. HTTP series - https://www.youtube.com/watch?v=8P6dG_K-a3I&list=PLopcHtZ0hJF1QZC8ThwdJqC-2aGhrpnbA&index=33
3. Master series - https://www.youtube.com/watch?v=Fg4spR6cdBQ&list=PLp50dWW_m40XTcxIaXVqO60LaIlyHWxDS


## Angular Material Study Material

Book series - https://code-maze.com/angular-material-series/

Youtube - https://www.youtube.com/playlist?list=PLp50dWW_m40V5ZNjLJiL1cMp1Fcww2V29

## Tips


1. To auto complete in VS code, install auto import extension to auto import the component and service imports

## Issues and Fixes


**PROBLEM:**

**Today i tried to setup my angular project and when i tried to run the ng serve i got below error**

Error: node_modules/@angular/platform-browser/platform-browser.d.ts:44:22 - error NG6002: Appears in the NgModule.imports of AppModule, but could not be resolved to an NgModule class.

This likely means that the library (@angular/platform-browser) which declares BrowserModule has not been processed correctly by ngcc, or is not compatible with Angular Ivy. Check if a newer version of the library is available, and update if so. Also consider checking with the library's authors to see if the library is expected to be compatible with Ivy.

44 export declare class BrowserModule {
                        ~~~~~~~~~~~~~

**SOLUTION:**

sudo npx ngcc

After this i try to run ng serve the app is up and running

---------------------------------------

**PROBLEM**

**Visual Studio Code always ask for permission to save files in Linux/Mac**

**SOLUTION**

Option 1

Using chown command ( Recommended)

cd location

sudo chown your_username your_project_directory

Option 2

Using the chmod -R 777 command ( It depends )

sudo chmod -R 777 your_project_directory_location

Example

Reference: https://dev.to/rahedmir/visual-studio-code-always-ask-for-permission-to-save-files-in-linux-140p



