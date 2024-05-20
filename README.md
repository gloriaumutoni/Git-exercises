# git-exercises
## Part 1: Refining Git History 
### Missing File Fix:
```
   24  git clone https://github.com/gloriaumutoni/git-exercises.git
   25  cd git-exercises/
   26  touch test{1..4}.md
   27  git add test1.md && git commit -m "chore: Create initial file"
   28  git add test2.md && git commit -m "chore: Create another file"
   29  git add test3.md && git commit -m "chore: Create third and fourth files"
   30  git status
   31  git log
   32  git add test4.md && git commit --amend
   33  history 0
   34  history
```
### Editing Commit History:
```
   35  git rebase -i HEAD~3
   36  git commit --amend
   37  git rebase --continue
   38  git rebase -i HEAD~3
   39  git rebase --continue
   40  git rebase -i HEAD~3
   41  git commit --amend
   42  git log
   43  git status
   44  git rebase -i HEAD~3
   45  git commit --amend
   46  git rebase --continue
   47  history
```
### Keeping History Tidy - Squashing Commits:
```
   48  git rebase -i HEAD~3
   49  history
```
