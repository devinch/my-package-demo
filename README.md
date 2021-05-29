## npm scope package demo

### sign in to npmjs.com (type username, password and email)
```
$ npm login
```


### publish scope public package
```
$ npm publish --access public
```

### publish to localµ
1. install Verdaccio and pm2
```
$ npm install verdaccio pm2 -g
```
2. start verdaccio with pm2
```
$ pm2 start verdaccio
```
3. add user and login
```
$ npm adduser --registry http://localhost:4873
```
4. nrm add registry
```
$ nrm add local http://localhost:4873
```
5. check current registry
```
$ nrm current

```
5. publish package
```
$ npm publish

```
> Tips: if npmjs.com had the same package name and same version, local will be refuse publish


### remove package in local 
```
$ npm unpublish <package-name> --force

```