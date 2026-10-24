lowkey makes sure u dont leak sm API keys or smth like that

installation:

1. Copy `git_sentinel.py` into the root of your Git repository.
2. Configure the pre-commit hook in `.git/hooks/pre-commit`:

```bash
#!/bin/sh
python git_sentinel.py
exit \$?
