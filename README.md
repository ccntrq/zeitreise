# zeitreise - A timetravel rebase tool

Make your commits go on a zeitreise

I like to rebase branches alot for a clean commit history. When you reorder your
commits like this they seem to appear in a weird order in some UIs. I always get
confused by this and have to look up the output of `git log` on my terminal.
This tool helps rebasing a branch and rewriting the commit timestamps in a way
that makes them appear in order.

*zeitreise* is the german word for timetravel.

# Usage

This is currently very fragile as I hacked it together in a few hours.
Don't hold me responsible for anything that happens using this.

You should reorder and edit your commits using `git rebase -i` as usual.
Afterwards you can use this tool to align the timestamps with the commit order.

```
./zeitreise master
```

This will take at least N seconds where N is the number of commits you are
rebasing.

# Status

## Version

0.0.1

## Planned Features:

- rewrite only commits where it is required
- try to obtain as much of the history as possible
