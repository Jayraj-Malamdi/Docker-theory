## Docker Theory

### 1) .dockerignore file

-----
```
# comment  : ignored
*/abc*     : files and directories having "abc" in its name is excluded.
abc?       : file or directories whose name starts with "abc" and has only one character after that are excluded.

*.md       : ignore all files with ".md" extensions
!README.md : all files with ".md" extensions are excluded EXCEPT README.md file.

*.md
!README*.md
README-secret.md

*.md
README-secret.md
!README*.md

- The difference b/w above two is that, in first all .md files are excluded except README files other then README-secret file.
WHEREAS 
in second all .md files are excluded and all README files are included, here second line has no effect.
BCOZ: placement of ! in .dockerignore determines its behaviour. 
```

