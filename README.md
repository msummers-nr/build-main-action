# build-main-action

This is the primary action invoked by every repository build, this is the only dependency that must be injected into each repository.

## TODO
- Fork anothrNick/github-tag-action and add a tag prefix option
- 
## Development
### Updating Release
- Commit local changes
- Push local changes
- Use `git log` to get the `HEAD` hash
- Update local tag to the `HEAD` hash
  - `git tag -f <TAG> <HEAD_HASH>`
- Push the updated tag to the remote
  - `git push --force origin <TAG>`
