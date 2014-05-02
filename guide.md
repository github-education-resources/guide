### 1. Sign up for GitHub

**If you already have a personal GitHub account, you can skip this step.**

GitHub has two types of accounts: [Personal and Organization][user-accounts]. To get started, you'll need to create a Personal account. Each individual user on GitHub should have exactly one Personal account. There's no need to maintain a separate account just for teaching, we'll use an Organization for that.

It's totally free to create an account, so go ahead and [sign up][signup].

### 2. Create an Organization for your class

**You must be logged in to GitHub to create an Organization account.**

A GitHub Organization represents a group of people working together, like a company or an open-source project. In this case, we'll use an Organization to represent your class in school. You can name your Organization anything you like. A common convention is to use some combination of the school name and course number. If you intend to repeat the course you may want to include the semester or year in the name.

[Create an organization][org-signup] for your class.

### 3. Give access to others

You'll probably want to add all co-teachers, teaching assistants, graders, etc. to the Owners team of the organization, so that they will have access to all your students' work.

You can read more about [Teams][help-team] and [access control][help-access-control] on GitHub Help.

### 4. Post your syllabus

You may want to create a public repository with your syllabus and assignment description(s). That way, students can see any changes made over time and create issues to ask for clarifications, and other teachers can collaborate with you to make your materials even better.

See [an example course repository](https://github.com/afeld/advanced_js).

### 5. Request free private repositories

**You only need the discount if you want to keep your students' code private.**

GitHub is free for open source and paid for private use. We're happy to offer free private repositories to teachers using GitHub with students in a classroom setting.

If you would like your students' code to remain private, [request a discount][discount]. Note these requests take up to a week to process, so please **do this in advance**.

### 6. Set up the repositories

**Your students need to sign up for GitHub before you can grant them access to your Organization.**

You have a couple options for how to organize the repositories for your students. You can use [`create_repos`][create-repos] action of our [teachers_pet][teachers-pet] tool, or do the following steps manually.

#### Individual projects

For each student:

1. Create a repository in the organization based on the student's name.
2. Create a team in the organization, matching the name of the repository.
3. Set that team to have `Push/Pull` permissions.
4. Add the student to that team.
5. Give that team access to the corresponding repository.

#### Group projects

For each group:

1. Create a repository in the organization.
2. Create a team in the organization.
3. Set that team to have `Push/Pull` permissions.
4. Add all of the group members to that team.
5. Give that team access to the corresponding repository.

### 7. Seed the repositories

If you have boilerplate code/files each student will need, you can create a starter repository locally, then [push][ref-push] it up to each student repository for that assignment. The [`push_repos`][push-repos] action in [teachers_pet][teachers-pet] automates this for you.

### 8. Get started with Git and GitHub

We have various resources available for Git and GitHub:

* [List of guides and tutorials][learning-materials] for learning how to use them
* [Open source training materials][teaching-materials] to you can use/customize for your classes
* [Git cheat sheet][cheat-sheet]

<!-- Links -->
[discount]: /discount
[help-team]: https://help.github.com/articles/how-do-i-set-up-a-team
[help-access-control]: https://help.github.com/articles/what-are-the-different-access-permissions#organization-accounts
[create-repos]: https://github.com/education/teachers_pet#creating-assignments
[teachers-pet]: https://github.com/education/teachers_pet
[push-repos]: https://github.com/education/teachers_pet#pushing-starter-files
[org-signup]: http://github.com/organizations/new
[signup]: https://github.com/signup
[user-accounts]: https://help.github.com/articles/what-s-the-difference-between-user-and-organization-accounts
[ref-push]: http://gitref.org/remotes/#push
[learning-materials]: https://help.github.com/articles/what-are-other-good-resources-for-learning-git-and-github
[teaching-materials]: http://training.github.com/materials/
[cheat-sheet]: /git-cheat-sheet-education.pdf
