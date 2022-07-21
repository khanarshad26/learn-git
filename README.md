# learn-git

Issue-1: 
MacBook-Air:learn-git apple$ git push origin master
error: src refspec master does not match any.
error: failed to push some refs to 'https://github.com/khanarshad26/learn-git.git'
MacBook-Air:learn-git apple$ git push
fatal: The current branch Branch_1 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin Branch_1

Ans:
The fatal: The current branch master has no upstream branch error occurs when you have not configured git in such a way that it creates a new branch on the remote. Therefore, you are only creating a new branch on the local computer.

You can fix the issue by typing:

    git push -u origin master

This will fix the error, but only for the current issue. The following is a permanent fix that will automatically create a remote branch:

    git config --global push.default current

The command above will fix the error and will always create a remote branch that tracks the local branch.

Change