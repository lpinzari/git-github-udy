# Introduction

Making commits to a repository can be nerve wracking. What if I make a mistake? What if I want to undo something I did in the past? Or what if I want to totally erase the last few commits because I'm positive they'll never be used?

That's exactly what we're going to look at. In this lesson we'll look at:

- `git commit --amend`: Alter the most recent commit. You'd want to do this if you **forget to include a file** in the commit or had a **typo in the commit message**.
- `git revert`: You provide it the SHA of the commit that you want reverted. Reverses given commit. The changes that were made in that commit are reversed. So **lines that were added in the commit will be deleted**. Don't worry though. We'll look at this in detail.
- `git reset`: You can actually **delete commits**. Erases commits. Now can just delete any commits. **You have to delte commits in order**. But this is a potentially dangerous command, because you are removing items from the repository.
