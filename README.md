# alpine-svn
## Description
Docker image for Subversion with WebDAV on Alpine Linux
## Usage:

Starting container with docker command:

````
docker run -d -P pikado/alpine-svn
```
The container start with the default account: davsvn (password: davsvn) and the default repository: testrepo

````
docker run -d -e SVN_REPO=repo -P pikado/alpine-svn
````
The container start with the default account: davsvn (password: davsvn) and the specified repository: repo

````
docker run -d -e DAV_SVN_USER=user -e DAV_SVN_PASS=pass -P pikado/alpine-svn
````
The container start with the specified account: user (password: pass) and the default repository: testrepo

````
docker run -d -e DAV_SVN_USER=user -e DAV_SVN_PASS=pass -e SVN_REPO=repo -P pikado/alpine-svn
````
The container start with the specified account: user (password: pass) and the specified repository: repo
