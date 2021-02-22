+++
title = "Documentation Style Guide"
draft = false

gh_repo = "chef-web-docs"

aliases = ["/style_guide.html"]

[menu]
  [menu.overview]
    title = "Docs Style Guide"
    identifier = "overview/community/style_guide.md Docs Style Guide"
    parent = "overview/community"
    weight = 40
+++

The Chef reference documentation is written using Markdown and built with Hugo.

We recommend that you use the conventions described in this guide when
contributing to the Chef reference documentation.

The HTML version of the doc set can be found at
[docs.chef.io](https://docs.chef.io).

## Building

To build the docs, run the command:

```bash
make serve
```

## Documentation Repo

The Chef reference documentation is located in: `https://github.com/chef/chef-web-docs`

- The `chef-web-docs` repo contains a `content` directory which holds most the Markdown files in the doc set.
- The `static/images` directory stores the image files used in the docs.
- The `config.toml` tells Hugo how to build the navigation menus and contains other Hugo settings. Don't modify this file.

In the past, the `chef-web-docs` repo contained documentation for prior
versions of Chef components. Currently, the repo is limited to the
current major versions of Chef components.

### DCO Sign-off

Chef Software requires all contributors to include a [Developer Certificate of Origin](https://developercertificate.org/) (DCO) sign-off with their pull request as long as the pull request does not fall under the [Obvious Fix](#obvious-fix) rule. This attests that you have the right to submit the work that you are contributing in your pull request.

For more information, review our [full DCO signoff policy](https://github.com/chef/chef/blob/master/CONTRIBUTING.md#developer-certification-of-origin-dco).

A proper DCO sign-off looks like:

`Signed-off-by: Tamira Bucatar <tbucatar@example.com>`

You can add a DCO signoff to your pull request by adding it to the text of your commit message, or by using the `-s` or `--signoff` option when you make a commit.

If you forget to add a DCO sign-off before submitting a pull request, you can amend your commit by entering `git commit --amend -s`. After that you'll likely have to force push your commit to github by entering `git push -f`.

See this [blog post](https://blog.chef.io/2016/09/19/introducing-developer-certificate-of-origin/) to understand why Chef started using the DCO signoff.

### Obvious Fix

Small contributions, such as fixing spelling errors, where the content is small enough to not be considered intellectual property, can be submitted without signing the contribution for the DCO.

Changes that fall under our Obvious Fix policy include:

- Spelling / grammar fixes
- Typo correction, white space and formatting changes
- Comment clean up
- Bug fixes that change default return values or error codes stored in constants
- Adding logging messages or debugging output
- Changes to 'metadata' files like Gemfile, .gitignore, build scripts, etc.
- Moving source files from one directory or package to another

To invoke the Obvious Fix rule, simply add `Obvious Fix.` to your commit message.

For more information, see our [Obvious Fix policy](https://github.com/chef/chef/blob/master/CONTRIBUTING.md#chef-obvious-fix-policy).

## Contact

See our [feedback](/feedback/) page if you have any questions or comments for the documentation team.
