Instructions on how to deploy of a React application onto GitHub pages

First step
create a new git repository . Note: the gitHub repository name should(optional) be the same as the react project name.

in the terminal change directory to the project folder and enter the following line:
git remote add origin https://github.com/{GitAccountName}/{RepositoryName}
commit and push all files to github:
git add -A
git commite -m "Initial commit"
git push -u origin main

Step 2
In package.json add:
"homepage": "https://{GitAccountName}.github.i/{RepositoryName}

step 3
npm install gh-pages --save-dev

sept 4
in package.json add the following under scripts tag:
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build",
    
step 5
npm run deploy

visit url 
