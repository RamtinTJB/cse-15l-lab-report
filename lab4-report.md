# Lab Report 4 - Vim

##### Log into ieng6
I typed `ssh cs15lfa23gz@ieng6.ucsd.edu<enter>`. Since I had previously stored my public ssh key on the ieng6 server, it didn't ask me for password and logged in automatically.

![ieng6 ssh login](images/lab4/lab4-ieng6-login.png)

##### Clone repo
I typed `git clone git@github.com:RamtinTJB/lab7-cse15l<enter>`. The reason this works is that I generated ssh keys on the ieng6 server and added my public key to my github account.

![git clone](images/lab4/lab4-git-clone.png)

Then I typed `cd lab<tab><enter>` to enter the directory I just cloned. The tab autocompleted the directory name to `lab7-cse15l`

![cd directory](images/lab4/lab4-cd-dir.png)

##### Run the tests (fail)

`bash te<tab><enter>` the tab autocompletes the filename to test.sh which is the script that runs the junit tests.

![test fail](images/lab4/lab4-test-fail.png)

As we can see, 1 test failed.

##### Fix the code
`vim List<tab>.j<tab><enter>` to open the file in vim. The first tab autocompletes to ListExamples and the second tab autocompletes to ListExamples.java

![vim open](images/lab4/lab4-vim-open.png)

`G` to go to end of the file `kkkkkk` to go 6 lines up `e` to go to the end of the first word (index1) `s2` to replace the last letter from 1 to 2 `<esc>` to exit insert mode.

![vim edit](images/lab4/lab4-vim-edit.png)

`:wq<enter>` to save the changes and exit vim

![vim close](images/lab4/lab4-vim-close.png)

##### Run the tests (succeed)

`bash te<tab><enter>` the tab autocompletes the filename to test.sh which is the script that runs the junit tests.

![test succeed](images/lab4/lab4-test-success.png)

As we can see, all tests passed this time.

##### Commit and Push

`git add Li<tab><enter>` to stage the file. The autocomplete works because that's the only file we changed `git commit -m "Fixed the bug"<enter>` to commit the staged change locally with the message "Fixed the bug" `git push<enter>` to push the changes to the remote.

![git](images/lab4/lab4-git.png)
