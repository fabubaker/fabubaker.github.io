To deploy changes to the `gh-pages` branch, run the following command:

```bash
git subtree push --prefix public origin gh-pages
```

`git subtree push --prefix ...` is used to collect commits that apply only to a
certain `prefix` (in the case above, the `public` directory) and push it to the
specified remote.
