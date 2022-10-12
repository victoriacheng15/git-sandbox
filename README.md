# git-sandbox

## Rebase and merge option

As the screenshot shows, it will show 3 commits ahead, 3 commits behind the main branch.

![image](https://user-images.githubusercontent.com/35031228/195426245-f6be0597-c194-4ee2-a6f0-1c71ad72ef4f.png)

how to make the development branch to be the same as main branch?

```
git switch development

git pull --rebase origin main

git push origin development --force/-f
```