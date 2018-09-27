## Merge repos with keeping the history

Adding `project-A` to `project-B`

```
cd ../project-B
git remote add project-A ../project-A
git fetch old-project
git checkout -b feature/merge-project-A
git merge -S --allow-unrelated-histories project-A/master
git push origin feature/merge-project-A
git remote rm project-A
```

## Pull with unrelated history
```
git pull ___ --allow-unrelated-histories
```

## Prevent push
```
git remote set-url --push origin no_push
```
