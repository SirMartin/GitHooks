# GitHooks
Some hooks that could be interesting

## commit-msg
Git commit-msg hook. If your branch name is following Jira like convention in the form **"ABCD-123-whatever"**, or
**"ABCD-123_whatever"**, it automatically adds the prefix **"ABCD-123"** to commit messages.

If you include **"#noref"** in the commit message, nothing will be added to the
commit message, and the **"#noref"** itself will be stripped.

### Installation

```cp commit-msg your_project/.git/hooks```

### Logging:
You can enable the logs to trace it, in case something is wrong. Just set to true the *LOG_ENABLED* constant.

### Testing:
*git init* a new repo, install the commit hook, and run:
```ruby .git/hooks/commit-msg testing```
