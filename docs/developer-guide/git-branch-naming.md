---
nav_exclude: true
---
## Git Branch Naming

For bugfix and hotfixes we don't always have an issue number so under these circumstances the ticket-number is optional.

- feature/[ticket-number]-[hyphenated ticket title]
```
 git checkout -b feature/123-hello-world
```
- bugfix/[ticket-number]-[hyphenated ticket title]
```
 git checkout -b 'bugfix/123-goodbye-bugs'
```
- hotfix/[ticket-number]-[hyphenated ticket title]
```
 git checkout -b 'hotfix/123-goodbye-bugs'
```