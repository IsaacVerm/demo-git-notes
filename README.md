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

Open `https://lite.datasette.io/?csv=https%3A%2F%2Fraw.githubusercontent.com%2FIsaacVerm%2Fdemo-git-notes%2Frefs%2Fheads%2Fmain%2Fdaily-notes%2Fdaily-notes.csv%3Ftoken%{token}#/data?sql=select+*+from+%5Bdaily-notes%5D+where+weather+like+%22%25rain%25%22`

`{token}` is displayed in URL when you open raw version of `daily-notes.csv`.
