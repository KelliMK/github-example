# A Project with Multiple Parties

## Pairs (or Stooges)

### Partner creating the project

1. One person create a project with a corresponding repository
1. Once the repository is created, add your partner(s) as Collaborators (Settings > Collaborators > [Enter username of partner])
1. Have your partner fork the repository and complete the following steps

### Partner forking the project

1. Clone the project to your machine
1. Add the original project as an upstream (`git remote add upstream https://github.com/[your-partners-username]/[name-of-the-original-project]`)

### Work flow

1. Before starting any work on code, create a feature branch (`git checkout -b some-descriptive-name`). Name it something describing the type of work you will be doing. (i.e. add-course-controller)
1. Make sure your work will not collide with your partners and begin making your tasked feature/fix/update etc. making meaningful commits as you go
1. Once you finish your feature, push your branch up to GitHub (`git add .`, `git commit -m "Finish course controller v1"`, `git push`)
1. Navigate to GitHub in your browser and go to the ORIGINAL project. There will be a yellow banner above the project files asking if you want to submit a pull request (PR)
1. Submit the PR and assign your partner to said PR (NEVER merge your own PR. Always have someone do a review of your code)
1. Once your partner approves your code they should merge the PR
1. Once the PR is merged, delete the feature branch both locally and remotely and pull from the master branch

#### If you are the partner that forked the project

1. instead of doing `git pull` from the master branch, you will instead switch to the master branch and execute the following:
	1. `git fetch upstream master`
	1. `git merge upstream/master master`

This will give you the updates from the original project.

Now, make a new feature-branch and start the process again.
