#### Install (Mac)
```
$ brew tap heroku/brew && brew install heroku
```

#### Login heroku account (Shell)
```
$ heroku login
heroku: Press any key to open up the browser to login or q to exit: 
Opening browser to https://cli-auth.heroku.com/auth/browser/XXXXXXXXXXXX
heroku: Waiting for login... ⣷
Logging in... done
Logged in as suhan.lee.k@gmail.com
```

#### Add git remote branch for deploy heroku 
```
$ git remote add heroku [HEROKU_GIT_URL]
```

#### Check git remote url
```
$ git remote -v
```

#### Deploy heroku using git hook
```
$ git push heroku master
```
