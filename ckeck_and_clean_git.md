
# Misc `git` commands


* This will clean all git commits, dangling messages and repair some problems:

```
git reflog expire --expire=now --all
git gc --prune=now
```

* When "Git refusing to merge unrelated histories" use the following option to `push` commend: `--allow-unrelated-histories`




