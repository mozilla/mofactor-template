# Contributing to {{ your app }}

At Mozilla we love our community and if you love what we're making but think it could somehow be better we would love to hear about it. Whether you want to report problems in our software or suggest (even provide) new features please use this guide to see what you need to do.

## Before you get started

All our code and issues are now on GitHub so if you're looking to contribute first make sure that you've got a GitHub account (they're free).

[Get a free GitHub account](https://github.com/signup/free)

## Reporting problems (bugs) or suggesting new features

1. **Check that it's not already been reported** - do a [quick search of our current issues][issues], if it has been but you have found additional information please leave this in the issues comments for us.
2. **[File a bug][new-issues]** - please make sure to provide all the relevant details so that it's clear that we know what the problem is; if you're unsure read our guide on [writing a good bug][good-bugs]. If you're suggesting new functionality please let us know exactly what you want (bonus points for wireframes/designs) and why. **[File a bug now][new-issues]**
3. **Assign some appropriate labels** - assign it the 'bug' or 'feature' label, for added bonus points assign any labels that will help us know what kind of skills are required to resolve it (for instance a front-end, accessibility bug or a server-side one)
4. **Watch out for bug updates** - we try and review bugs on a daily basis, if you see that we've asked for further information or have asked for confirmation (you'll get an email from GitHub if we do) that we've fixed the bug please help us out by answering as quickly as you can.

## Contributing code

We're always very happy to accept pull requests on any of our open issues, they're a fantastic help. We all ensure that we follow the same process, so to have your code merged in please do as we do!

1. **Assign a bug to you** - please assign the bug you're looing to fix to yourself, this will stop anyone else from working on it. If there isn't an open issue for the code you're looking to provide please use the guide above to create a new bug to assign yourself to.
2. **Set up your local development environment** - get a development server set up on your machine, [use our handy guide][dev-environment]
3. **Create a new feature branch** - for each issue work in a branch off our development branch

    ```bash
    git checkout development
    git pull upstream development
    git checkout -b <topic-branch-name>
    ```
4. **Do your work** - make sure to adhere to the coding conventions used throughout a project (indentation, accurate comments, etc.). Please update or include any documentation that is relevant to the change you're making.
5. **Prepare your pull request** - we like pull requests to be just the 1 atomic commit ([use an interactive rebase](https://help.github.com/articles/interactive-rebase)), once you've sorted that please ensure that you're pulling in the latest code incase anything has changed that might effect the work that you've done.

    ```bash
    git rebase -i HEAD~<number-of-local-commits>
    git pull --rebase upstream development
    ```

    If there are any conflicts please resolve them - if you need to ask questions jump into #mofodev on irc.mozilla.org

6. **Push your local branch up to your GitHub fork** 

    ```bash
    git push origin <topic-branch-name>
    ```
7. **[Open a pull request](http://help.github.com/send-pull-requests/)** - include the words 'fixes #<issue-id>' in the title and provide a clear description. Add the label 'needs-review' to the newly openned bug on github (each new pull request opens up a new bug)
8. **Prepare for code review** - we code review all pull requests, please keep a look out for the issues progress and be ready to fix-up or answer any comments we may have and to confirm your code is working as expecting when merged into and previewed on our [development server][dev-server].

Once your code has gone through review and has been merged successfully into development it'll soon make it's way to production. Please fix as many issues as you would like :)

[issues]: https://github.com/mozilla/mofactor-template/issues
[new-issues]: https://github.com/mozilla/mofactor-template/issues/new
[good-bugs]: #
[dev-environment]: https://github.com/mozilla/mofactor-template/wiki/Installation-and-Configuration
[dev-server]: #
