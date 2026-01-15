# demo-git-notes

Show scalable way of keeping track of daily notes.

## Concatenate all notes

```
cat daily-notes/* > summary-daily-notes.md
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