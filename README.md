PEP8-Commit-Hook
================

Originally forked from ``https://gist.github.com/810399``

Altered by @gaker to ignore the Django manage.py file, and any schema
migration files created by South.

To use this file on a project by project basis, create a file in
project_root/.git/hooks called pre-commit.  

```bash
$ chmod +x project_root/.git/hooks/pre-commit
```

Additionally, don't forget to ``pip install pep8``

PEP8 is meant to be ignored when it makes most sense. If you think it
makes sense to ignore something like a 79 character line, the hook can be
bypassed with:

```bash
$ git commit --no-verify
```
