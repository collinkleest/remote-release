### Release notes
List current tags
```bash
git tag
```

1. Go to https://github.com/collinkleest/remote-release/releases
2. Click "Draft a new release"
3. Version the release with a tag (i.e. v1.0.2)
4. Run `git fetch --tags`
5. Point old tag at desired tag (i.e. `git tag -f v1 v1.0.2`) this will effectively point `v1` to `v1.0.2`
6. Force push `git push -f origin --tags`