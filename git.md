# general git flow

## downloading
Go to location where you want the file downloaded
```
git clone "https.... reponame.git
```

## Updateing
```
git pull 
git add filenameToAdd
git commit -m 'this is what I did'
git push
```
1. git pull gets the latest version from remotes
2. git add = adding the file you want to change to your list of changes
3. git commit -m, locally setting the new state of the files you want to push with a message
4. git push, pushing the change to the remotes (in most cases, github)

## Get Git Revision
```git rev-parse HEAD```
## git clean
```-dfx ```

## Revert a single file back to state on a different brance
```git checkout <branchThatHasTheStateYouWant> <full-path-to-file>\file.txt
git checkout main <full-path-to-file>\file.txt
```
