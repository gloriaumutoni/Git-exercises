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
