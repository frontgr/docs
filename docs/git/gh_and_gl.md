# Как одновременно работать с Github и Gitlab

Для этого нужно настроить git remotes, удаленные репозитории для Github и Gitlab: 

```yaml
git remote add github <GitHub repository URL>
git remote add gitlab <GitLab repository URL>
```


Далее можно посмотреть, все ли корректно добавилось: 

```yaml
git remote -v
```

Чтобы делать push/fetch/pull/etc. в удаленные репозитории, можно делать это отдельно: 

```yaml
git push gitlab main 
```

Эта команда будет пушить в удаленный репозиторий gitlab в ветку main. А вот так можно сделать push во все удаленные репозитории: 

```yaml
git push --all
```
