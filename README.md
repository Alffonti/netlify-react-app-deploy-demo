# How to deploy a React app with Netlify

This project shows how to deploy a React app with Netlify.

## Create a React App
```
npx create-react-app netlify-react-app-deploy
cd netlify-react-app-deploy
npm run build
```

## Install Netlify CLI and Deploy
```
npm install netlify-cli -g (it will install it globally)
netlify deploy
```

After entering netlify deploy, choose “Create & configure a new site”.

## Create Github repo and push up current project
Create a new repository on the command line 
```
git add -A
git commit -m 'Added local Netlify foler'
git branch -M main
git remote add origin https://github.com/Alffonti/netlify-deploy.git
git push -u origin main
```

## Link Netlify App to GitHub
Select "Build and Deploy" in "Site Settings" and, then, select "Link site to Git"
Choose the recently created repository and, that's all, your site is published.

### Acknowledgements

- [Gene Campbell III](https://levelup.gitconnected.com/how-to-deploy-a-react-app-with-netlify-set-up-continuous-deployment-via-github-53859dcdaf40)
- [Netlify Blog](https://www.netlify.com/blog/2016/07/22/deploy-react-apps-in-less-than-30-seconds/)
