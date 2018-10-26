# Changing the fetch/push URL for a remote

After cloning a fork of a remote, you may want to set the fetch URL for your origin remote to be the source's URL. This makes for easy updates to your local copy.

```bash
git remote set-url origin --fetch /path/to/source.git
```

Likewise, you can change the push URL.
```bash
git remote set-url origin --push /path/to/fork.git
```
