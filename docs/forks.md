To have students complete assignments using forks:

### 1. Create the repositories

**Create one repository per assignment**. Include any boilerplate files your students will need to get started.

If you'd prefer that your assignments or students' work isn't publicly visible, [request private repositories][private-repos] to use for your class. You will need one private repository per assignment.

### 2. Give students read-only access

**If your repositories are public, you can skip this step.**

If your course materials are in private repositories, students will need read-only access to them. Create a `students` team with "read access" and [add each student to it][add-to-team]. Then, give that team access to all repositories that they will need.

[Read more about access control][help-access-control].

### 2. Completing assignments

Your students then follow these steps for each assignment:

1. To start, [**fork** the repository][forking].
1. [**Clone**][ref-clone] the repository to your computer.
1. Modify the files and [**commit**][ref-commit] changes to complete your solution.
1. [**Push**][ref-push]/sync the changes up to GitHub.
1. [Create a **pull request**][pull-request] on the original repository to turn in the assignment.

You may consider making a context-specific copy of these steps in your syllabus or assignment description – grab [the markdown][raw].

### 3. Reviewing assignments

Once created, you can then do code review with line-by-line feedback directly within the pull request. If you allow your students to submit corrections, they can push fixes up to their forks, which will be reflected in the pull request.

Since you don't want any solutions in the original assignment repository, you should leave the pull request unmerged. When you're finished giving feedback, you can close the pull request and leave a :+1: (`:+1:`) in a final comment.

<!-- Links -->
[private-repos]: /guide/private_repos
[add-to-team]: https://help.github.com/articles/adding-organization-members-to-a-team
[help-access-control]: https://help.github.com/articles/what-are-the-different-access-permissions#organization-accounts
[forking]: https://guides.github.com/activities/forking/
[ref-clone]: http://gitref.org/creating/#clone
[ref-commit]: http://gitref.org/basic/#commit
[ref-push]: http://gitref.org/remotes/#push
[pull-request]: https://help.github.com/articles/creating-a-pull-request
[raw]: https://raw.githubusercontent.com/education/guide/master/docs/forks.md
