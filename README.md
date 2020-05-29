## To deploy react app using Github:

1. npm install
2. npm install gh-pages --save-dev
3. Add properties to package.json file as following:
    - Add at the start "homepage": "https://{username}.github.io/{repo-name}"
    - In the existing scripts property add:
    "scripts":{
           // ...
          "predeploy": "npm run build",
          "deploy": "gh-pages -d build"
          }
4. git init
5. git remote add origin {repo-address}
6. npm run deploy
7. git add .
8. git commit -m "Your message"
9. git push origin master

###### The above steps will help you to deploy React app.
