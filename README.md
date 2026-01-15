# demo-git-notes

Show scalable way of keeping track of daily notes.

## Concatenate all notes

```
cat daily-notes/*.md > daily-notes/daily-notes.md
```

## Keyword search

```
cat daily-notes/* | grep rain
```

## Go back to older version

Back to original version before modifications in this case:

```
git log --oneline
git checkout 57085ec
```

## Go back to last commit

```
git switch -
```

## Daily notes as database approach

Import CSV into [Datasette Lite](https://lite.datasette.io/).