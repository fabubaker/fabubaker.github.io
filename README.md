To deploy changes to the `gh-pages` branch, run the following command:

```bash
git subtree push --prefix public origin gh-pages
```

`git subtree push --prefix ...` is used to collect commits that apply only to a
certain `prefix` (in the case above, the `public` directory) and push it to the
specified remote.

As a result, there is never a need to directly modify the `gh-pages` branch, it
will automatically be updated with the `git subtree` commanded (albeit with different commit ids compared to `master`).
