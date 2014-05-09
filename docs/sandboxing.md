To set up assignments using the sandboxing method (a.k.a. "fake forks"):

### 1. Get an upgraded plan

See our [guide][private-repos] on getting private repositories to use in your class. You will need one private repository per student per assignment.

### 2. Set up the repositories

You have a few options for how to organize the repositories for your students. We have a command-line tool called [teachers_pet][teachers-pet] that automates some of these steps. You can use the [`create_repos`][create-repos] action to create the repositories, or do the following steps manually.

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

If you have boilerplate code/files each student will need, you can create a starter repository locally, then [push][ref-push] it up to each student repository for that assignment. The [`push_repos`][push-repos] action in [teachers_pet][teachers-pet] automates this for you.

<!-- Links -->
[private-repos]: /guide/private_repos
[create-repos]: https://github.com/education/teachers_pet#creating-assignments
[teachers-pet]: https://github.com/education/teachers_pet
[push-repos]: https://github.com/education/teachers_pet#pushing-starter-files
[ref-push]: http://gitref.org/remotes/#push
