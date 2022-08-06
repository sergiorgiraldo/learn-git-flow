# learn-git-flow
recipe
* copy from repository `git-flow-sem-ver` to `.git\hooks`
* in the root do `git flow init`
* update remote `git push origin develop`
* start with `git flow feature start whatever`
* code, commit, push. dont forget to create file in root, named *VERSION* with content *0.0.0* 
* end with `git flow feature finish`
* release with `git flow release start major`
* change VERSION file (see new version number on the output of the command)
* commit/push VERSION (and others files, if any)
* end release with `git flow release finish 1.0.0` (1.0.0 or whatever version number)
* update remote, checkout develop and `git push`
* update remote, checkout main and `git push`
