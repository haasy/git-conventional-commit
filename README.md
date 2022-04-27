#Git with Conventional Commits
The `.gitmessage` template can be used as a commit template for a repository by running
```bash
git config commit.template "<path_to_.gitmessage>"
```
in it.

To enforce Conventional Commits the `commit-msg` bash script can be used by placing it in the hooks directory (`<repo>/.git/hooks`) of the repository for which it should be enfored.

The script filter out any comments and checks the first line of the commit message using a regex. If changes to the format are desired the regex in the script can be adjusted.