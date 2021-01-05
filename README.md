# git-rstash
Transfer your Git stashes to and from remotes with ease!

## Usage

Place or link `git-rstash` somewhere on your `PATH`, then:

```
usage: git rstash list [<user>] [<remote>]
   or: git rstash pull [<user>] [<remote>]
   or: git rstash push [<remote>]
   or: git rstash purge [<user>] [<remote>]

advanced usages:
git rstash list-all [<remote>]
git rstash list-sha [<user>] [<remote>]
git rstash list-sha-all [<remote>]
git rstash pull-all [<remote>]
git rstash pull-only [<user>] [<remote>]
git rstash pull-only-all [<remote>]
git rstash push-one <stash> [<remote>]
git rstash purge-all [<remote>]
git rstash drop <stash> [<remote>] ['\''y'\''|'\''n'\'']
git rstash import <SHA>
git rstash import-all
```

where `<stash>` is a stash number, `<SHA>` is a (short or long) SHA commit hash, and `[<remote>]` is an (optional) remote to operate on.

By default, `git-rstash` uses `origin` as the remote.  Stashes are saved both remotely and locally to `refs/stashes/<SHA>`.

See [my Stack Overflow answer](https://stackoverflow.com/a/61356308/2747593) for more details.
