# Contribution guide
## Would you like to contribute?
Whether you're new to GitHub and looking for experience or just want to help out, we welcome your contribution. This project is meant to give contributors an introduction into the world of code collaboration as well as basic web development.

If you haven't already, join the conversation in the \#team-project channel of [our Discord server](https://discord.gg/SXJm486). Let us know what you want to add to this project. If you need help with making a contribution, feel free to ask.

Also, check out our [roadmap](https://docs.google.com/document/d/1kYv8QNoU3tTTwtrgt773sBLYIhpiNiZ9Jdm_FEu6AH4/pub) for this little project for an overview of what we've got planned.

## Forking and cloning
In order to submit changes to the Campfire Coders repository, you'll need to fork the repository and maintain a local copy of it. Check out [GitHub's guide to forking](https://help.github.com/articles/fork-a-repo/) for info on how to do that.

If you followed the guide (replacing the example repo with Campfire Coders repo), you should have two copies of the Campfire Coders repository:
- one in your GitHub account (`github.com/your-username/campfirecoders.github.io`)
- one local copy within a folder called `campfirecoders.github.io`.

Your local repo's `upstream` should be set to `https://github.com/campfirecoders/campfirecoders.github.io.git`, like the example in [this section](https://help.github.com/articles/fork-a-repo/#step-3-configure-git-to-sync-your-fork-with-the-original-spoon-knife-repository) of the guide.

## Working with a local copy
**Note:** Make sure your master branch is synced to the original Campfire Coders repository and that you are working on a separate branch before you start making changes to your local repository. Here are the steps to follow:

1. Open Git Shell and navigate to the repository
2. Make sure you are on the master branch, using `git status`:

   ```
   On branch master
   Your branch is up to date 'origin/master'
   ```
   
3. If you are not on master, use `checkout master`
4. Do a `pull` with rebase against `upstream`:
   `git pull --rebase upstream`
   This will sync your local repo with the original master without making an additional commit locally.
5. Create a branch off of master with: `git checkout -B branchname` replacing `branchname` with the name of your new branch. Use a name that gives an idea of what feature or fix you are going to implement such as `navbar-styling`.
6. Now you're ready to make some changes to your local files!

## Pushing changes to your GitHub fork
Alright, so you've made some changes in your local copy of the Campfire Coders repo, tested your changes on your browser and you're ready to submit those changes for all to see. Now what?

1. Run `git status` and you'll see all the files you've changed and haven't staged yet.
2. Add your changed files to be staged with: `git add path/to/filename.ext` You can also do: `git add .` to add all unstaged files. Check `git status` before doing adding all unstaged files, as you may end up staging some unwanted files.
3. Commit your edits: `git commit -m "commit description"`
4. [Squash your commits](http://gitready.com/advanced/2009/02/10/squashing-commits-with-rebase.html), if there are more than one.
5. Push your commit to your fork on GitHub: `git push -u origin branch-name`. The branch name should be the same as the branch you were working with.

## Submitting a pull request
Once you've got your changes pushed to your fork of the Campfire Coders repo on GitHub, it's time to [submit a pull request](https://help.github.com/articles/creating-a-pull-request/).

The name of your pull request (PR) should give us an idea of the changes you've made, such as `add styling to navbar`.

If your PR is meant fix a specific issue, add `closes #123` in the description of your PR where `#123` is the issue number. This will allow GitHub to automatically close the issue once your PR is merged

If your PR is not accepted, we'll let you know what changes need to be made.