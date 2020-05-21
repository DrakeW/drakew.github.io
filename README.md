# Some deployment notes

Since github pages only allows to deploy `master` branch, we will push the content in the `public` directory as a subtree to master, and use `develop` branch as the source code branch.

To push built artifacts to master, run

```{bash}
hugo -D  # to build
git subtree push --prefix public origin master
```
