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
### Splitting a Commit:
```
   50  git reset HEAD~
   51  git add test3.md
   52  git commit -m "created third file"
   53  git add test4.md
   54  git commit -m "created fourth file"
   55  git log
   56  history
```
### Advanced Squashing:
```
  57  git rebase -i HEAD~3
  58  history
```
### Dropping a Commit:
```
   59  touch unwanted.txt
   60  git add .
   61  git commit -m "Unwanted commit"
   62  git rebase -i
   63  git log
   64  history
```
### Reordering Commits:
```
   65  git rebase -i
   66  git rebase -i HEAD~3
   67  git rebase -i HEAD~2
   68  history
```
