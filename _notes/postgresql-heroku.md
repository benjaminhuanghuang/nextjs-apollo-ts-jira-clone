Install Heroku CLI
```
curl https://cli-assets.heroku.com/install-ubuntu.sh | sh

heroku update

heroku -v
```

Add the Heroku remote by using UI Heroku Dashboard -> myherokuapp or Your App Name -> Deploy Section 
or  run command
```
heroku login

heroku git:remote -a myherokuapp
```


Deploy
```
git add.

git commit -m "First Commit"

git push heroku master
```

For eact app, add an extra build back in the `settings section` of the Heroku app
```
https://buildpack-registry.s3.amazonaws.com/buildpacks/mars/create-react-app.tgz
```


Logs
```
heroku logs --tail
```