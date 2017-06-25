# Public Key Repo

## How to use

1. Clone this repo or fork it.
2. Copy the pre-commit file into .git/hooks and make sure it's executable.
3. Update or add a public key. Make sure all key filenames end with `\_rsa.pub`. (It should go without saying, but never put a private key in here.)
4. Commit your change. The pre-commit hook will prevent your commit if anything is invalid.

## Pre-commit hook

1. Goes in .git/hooks and must be executable.
2. Checks that keys are valid.
3. Combines all the keys into a `combined\_rsa.pub` file.
4. Stages that file for any commit where keys change.

