__Lab 7 Steps 4 - 9__

*when I fixing the coding format it wouldnt work, I have everything with <> under `<enter>` for example but when i print it wont print right*
4) Logged into ieng6
   - ssh cs15lfa23oq@ieng6.ucsd.edu + `<enter>`

![Image](logging_in_without_password.png)
5) clone the repository using the SSH URL
  - git clone git@github.com:noehparrales/lab7.git + `<enter>`
![Image](git_clone.png)
6) test the code
  - bash test.sh + `<enter>`
![Image](failed_test.png)
7) edited code using vim
  - first I had to use the command: vim ListExamples.java + `<enter>`
  - then I pressed `<j>` 10 times to go to line where one of the problems is at, pressed `<l>` 16 times to go right
  - the first problem was that result.add(0,s) has the 0 which makes the first test case fail 
  -  pressed `<x>` ttwice to delete the unwanted characters
  - from there, I pressed `<j>` 29 more times to go to the next code issue, and `<h>` 6 times to go left
  - the next issue is that index1 should be index2
  - go to the unwanted character and press `<x>`
  - then clicked `<i>` to add text, replaced it with a 2, then pressed `<esc>` to go back to normal mode.
  - lastly typed the command `<:wq>` + `<enter>`to save the edits 
![Image](editing_vim.png)

8) retest code
   - used bash test.sh + `<enter>`
![Image](good_test.png)

9) commit and push code
    - I used the command `git add .` + `<enter>` so all changes I made to any existing files can be commited, then used the command `git commit -m "working code" ` + `<enter>` which saves the changes, then used `git push` + `<enter>` which uploads the changes from the local repository to the remote repository. 
![Image](good_commit.png)
![Image](good_push.png)
