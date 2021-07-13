# Contributing Guidelines

If you wish to contribute changes to the MEI website, you can edit the files directly on GitHub. The website is written in a dialect of Markdown called [kramdown](https://kramdown.gettalong.org/quickref.html).

[//]: # (In the guidelines you will see links to "Edit this section". Clicking on this will open up an editor in GitHub, where you will be able to click on the 'pencil' to edit the text of the section.)

When you are finished, you can then “Propose a file change”, where you can write a brief summary of your changes and their motivations, and then “Create a Pull Request”, which will alert the MEI Technical Team of your proposed change. If there are any questions or problems with your suggested change, a discussion can happen on the Pull Request, and then it will be merged into the website.

In some cases you will see special markup that will create automatic contents. If you need help with this Markdown, the Technical Team will be happy to help.

For complex contributions, you may wish to get the website running on your local machine, and submit a larger Pull Request. This will be explained in the next section.

## Editing the website locally

If you wish to contribute significant changes, you will likely want to checkout the code from this repository and work on it locally. To do so you will need to install Jekyll, which requires Ruby. This guide will assume you have a functioning Ruby environment, with the `gem` and `bundle` commands available. If you do not, please follow [these instructions](https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/#requirements) on getting these set up.

### Step 1: Fork the website

You should fork the website into your own account using the “Fork” button on GitHub. This will make a copy of the music-encoding.github.io repository which you can edit.

### Step 2: Clone to local machine

In order to work with the repo offline you neet to clone the code to your local machine, e.g. by clicking the green “Code” button at the top and following one of the corresponding instructions.

### Step 2: Create a new branch

Create a new branch for your changes on your local Git repository. You should make it a descriptive name, like ‘feature_new-project’, ‘fix_broken-links’ or similar.

### Step 3: Test your changes locally

In case you have made bigger changes you might want to make sure the website behaves as expected before committing to your fork and opening a pull request against the upstream repository.

In order to do so you have to run the Jekyll locally (for dtails on Jekyll visit (https://jekyllrb.com)[https://jekyllrb.com]). Jekyll is the engine behind Github Pages, which is used to host the MEI website.

There are several options to do so, two of which are described within this repository:

1. [Install Jekyll natively](contributing/jekyll_native.md) on your local machine
2. [Use a Docker Container](contributing/jekyll_docker.md) to execute Jekyll

### Step 5. Make your changes and commit

You should now be able to make your changes. Try to keep your commits as ‘atomic’ as possible; that is, commit only the changes necessary for a given set of functionality. Avoid large commits that change a lot of things, as this makes it harder to review your changes for unintended side effects and potential problems.

### Step 6. Propose a Pull Request

Once all of your changes have been committed and pushed to your fork, you can propose a change to the main music-encoding.github.io repository by opening a [Pull Request](https://help.github.com/articles/about-pull-requests/). This will alert the Technical Team that you have a change you wish to contribute. The 'Technical Team will review your changes and may ask for modifications or clarification in the Pull Request. Once your changes have been reviewed and accepted, they will be merged in and will then be available on the website.

### Step 7. Delete your local branch (optional)

When your pull request has been accepted, it is then safe to delete the branch that you created in Step 2. This will ensure you do not have older branches around that get progressively outdated.
