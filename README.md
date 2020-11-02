# rails-template

A rails application template with some personal tweaks.


## Usage

To start a new rails project based on this template, you clone this repository:

```
$ git clone https://github.com/hugopeixoto/rails-template your-app
$ cd your-app
```

You can drop features you don't want by rebasing the git history interactively:

```
$ git rebase -i --root
```

You can drop the git history if you don't want my name and email polluting your
repository:

```
$ rm -rf .git && git init
```

Finally, you'll probably want to change the README file.


## Features / changes

* No spring, turbolinks, action-cable, action-mailbox, or webpack
* postgresql with uuids by default
* UTC timezone
* dotenv
* pundit
* rubocop
* factory-bot
* faker


## Development

I'm still not sure how to handle project updates. The way I'm planning on doing
it for now is to squash any fixes to the commit that introduces that change,
instead of continuously adding new commits. This allows users to drop commits
with features that they'd like to skip.

If this evolves into something that's not simply a rails app template, I might
change this to use a regular git workflow.

I will accept any PRs and handle rebasing if it's fixing something or
introducing a feature that I personally would use.

## See also

[Thoughtbot's suspender project](https://github.com/thoughtbot/suspenders) is a
similar idea but way more complete, you might want to check it out.
