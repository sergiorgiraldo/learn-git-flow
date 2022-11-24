# learn-git-flow

## recipe
## setup - once
* copy from repository `git-flow-sem-ver` to `.git\hooks`
* in the root do `git flow init`
* update remote `git push origin develop`

## lifecycle - many
* start with `git flow feature start whatever`
* code, commit, push. dont forget to create file in root, named *VERSION* with content *0.0.0* 
* end with `git flow feature finish`
* release with `git flow release start major` (major or minor)
* VERSION file is updated automatically
* commit/push
* end release with `git flow release finish 1.0.0` (1.0.0 or whatever version number)
* `git push` develop
* update main with pull request
  * checkout develop
  * gh pr create
  * gh pr merge
