# git-sandbox

## Rebase and merge option

As the screenshot shows, it will show 3 commits ahead, 3 commits behind the main branch.

![image](https://user-images.githubusercontent.com/35031228/195426245-f6be0597-c194-4ee2-a6f0-1c71ad72ef4f.png)

how to make the development branch to be the same as main branch? If you open a PR to merge changes from development to main branch.

```
git switch development

git pull --rebase origin main

git push origin development --force/-f
```

## Sqush and merge option

Forgot to take the screenshot but it is similar to rebase and merge. Instead, sqush and merge will show as one commit ahead of main and a dropdown menu if there are more than 1 commit.

![image](https://user-images.githubusercontent.com/35031228/195432673-bff2c015-c684-4213-819f-5313b845c4ec.png)


## Overall

To merge development to main, maybe it is the better way.

```
git switch main

git pull --rebase origin development

git push origin main
```

This should update your main branch with latest change from development. Maybe ideal, but depend on the team.

OR

Always run this first

``` 
git fetch && git pull origin main
```

```
```