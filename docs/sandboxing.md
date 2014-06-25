To set up assignments using the sandboxing method (a.k.a. "fake forks" or [duplicated repositories][help-duplicate]):

### 1. Get an upgraded plan

See our [guide][private-repos] on getting private repositories to use in your class. You will need one private repository per student per assignment.

### 2. Set up the repositories

You have a few options for how to organize the repositories for your students. We have a command-line tool called [teachers_pet][teachers-pet] that automates some of these steps. You can use the [`create_repos`][create-repos-action] action to create the repositories, or do the following steps [manually][help-duplicate].

#### Individual projects

For each student:

1. Create a repository in the organization based on the student's name.
1. Create a team in the organization, matching the name of the repository.
1. Set that team to have `Push/Pull` permissions.
1. Add the student to that team.
1. Give that team access to the corresponding repository.

#### Group projects

For each group:

1. Create a repository in the organization.
1. Create a team in the organization.
1. Set that team to have `Push/Pull` permissions.
1. Add all of the group members to that team.
1. Give that team access to the corresponding repository.

### 3. Seed the repositories

If you have boilerplate code/files each student will need, you can create a starter repository locally, then [push][ref-push] it up to each student repository for that assignment. The [`push_files`][push-files] action in [teachers_pet][teachers-pet] automates this for you.

For the assignment instructions, use one of these two recommended options:

* Create a canonical repository with instructions, in the syllabus repository, or in one dedicated to the assignment.  This gives a canonical source for students to refer to.  If you do create a README in each student's repository, add a link to the canonical instructions.
* Open issues in each student's repository for them to complete.  The [`open_issue`] command in [teachers_pet][teachers-pet] automates this for you.

<!-- Links -->
[help-duplicate]: https://help.github.com/articles/duplicating-a-repository
[private-repos]: /guide/private_repos
[create-repos-action]: https://github.com/education/teachers_pet#creating-assignments
[teachers-pet]: https://github.com/education/teachers_pet
[push-files]: https://github.com/education/teachers_pet#pushing-starter-files
[ref-push]: http://gitref.org/remotes/#push
[open-issue]: https://github.com/education/teachers_pet#opening-issues
