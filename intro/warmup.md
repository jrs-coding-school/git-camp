# Warmup

These warmups assumes you have the following software installed on your local machine.  If you have not already done so, complete [Exercise 1: Install and Setup](/intro/1).

- git
- NodeJS
- Atom

## Warmup 1: Find Tom and Trip

- I like to store all my coding projects within the same parent directory that I call my "code home" directory.  Using terminal , make sure you are in your "code home" directory. For the remainder of this warmup, I will assume my "code home" directory is **jrs/code**.  Your "code home" directory will vary.  

  > Tip:  If you get lost, you can always drag and drop a folder from the Mac's Finder application into Terminal.

  ```
  $ cd jrs
  $ cd code
  ```

- One you are within your "code home" directory, enter the following command to _clone_ a specific GitHub repository named **whereIsTomAndTrip**.  This command will bring down several files and folders from GitHub.com (internet) to your local machine.  

  ```
  $ git clone https://github.com/jrs-innovation-center/whereIsTomAndTrip.git
  ```

Cloning the repostory creates a subdirectory named **whereIsTomAndTrip**  within your "code home" directory.

- From you "home directory", use the `cd` command to change to the **whereIsTomAndTrip** folder/directory.

  ```
  cd whereIsTomAndTrip
  ```

Two image files, one for Tom and another for Trip, exist within the  **whereIsTomAndTrip** folder.  Use the following commands to locate each image file. Pay attention to the clues.

Use the `cd` command to change to another directory.  Ex: `cd a`.

```
cd  
```


## Warmup 2: Command Line Calisthenics

Create the following directories at the command line.  We will delete all of these folders, etc. when were done.

- At the command line, make sure you are in your "code home" directory.
- Within your "code home" directory, create a directory named 'delete-me' via `mkdir delete-me`.

  ```
  \your-code-home-will-vary\
  \your-code-home-will-vary\delete-me\
  ```
- Change directory `cd` to the `delete-me` directory.

  ```
  \your-code-home-will-vary\delete-me\
  ```

- Within the `delete-me` directory, create the following directory structure/tree using the terminal:

  ```
    \your-code-home-will-vary\delete-me\node-project-a
    \your-code-home-will-vary\delete-me\node-project-b

    \your-code-home-will-vary\delete-me\node-project-a\static\assets\images
    \your-code-home-will-vary\delete-me\node-project-a\static\assets\style
    \your-code-home-will-vary\delete-me\node-project-a\dal

    \your-code-home-will-vary\delete-me\node-project-b\static\assets\images
    \your-code-home-will-vary\delete-me\node-project-b\static\assets\style
    \your-code-home-will-vary\delete-me\node-project-b\dal
  ```
  - Open the `node-project-a` and `node-project-b` project folders using your atom code editor.  Inspect your file structure against the example above.

  - Within the directory structure/tree create the following files using `touch <filename>`.  

    > Windows users can use atom to create new files, if `touch` is not available.

    Here are the files:

    ```
    \your-code-home-will-vary\delete-me\node-project-a\index.js
    \your-code-home-will-vary\delete-me\node-project-a\readme.md

    \your-code-home-will-vary\delete-me\node-project-b\index.js
    \your-code-home-will-vary\delete-me\node-project-b\readme.md

    \your-code-home-will-vary\delete-me\node-project-a\dal\index.js
    \your-code-home-will-vary\delete-me\node-project-b\dal\index.js
    ```

  - Within each of the following project folders, use `npm init -y` to initialize and create the beginnings of a nodeJS project.

    ```
    \your-code-home-will-vary\delete-me\node-project-a
    \your-code-home-will-vary\delete-me\node-project-b
    ```
