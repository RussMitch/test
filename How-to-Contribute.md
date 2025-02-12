# Contributing to GPSSample Code
There are many ways to contribute to the GPSSample project: logging bugs, submitting pull requests, reporting issues, and creating suggestions.

After cloning and building the repo, check out the [issues list](https://github.com/GPS-Sample/GPS-Sample/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue). Issues labeled [`help wanted`](https://github.com/GPS-Sample/GPS-Sample/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22) are good issues to submit a PR for. Issues labeled [`good first issues`](https://github.com/GPS-Sample/GPS-Sample/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22) are great candidates to pick up if you are in the code for the first time. If you are contributing significant changes, or if the issue is already assigned to a specific month milestone, please discuss with the assignee of the issue first before starting to work on the issue.

## Prerequisites

In order to build the application, you'll need to:

* Download and install [Android Studio](https://developer.android.com/studio)
* Clone the repo
* Add your [MapBox](https://www.mapbox.com/) license secret key to the local.properties file:

   MAPBOX_DOWNLOADS_TOKEN=YOUR-SECRET-KEY
  
* Build/Run the application on your Android 8+ device

## Build and Run

If you want to understand how GPSSample works or want to debug an issue, you'll want to get the source, build it, and run the tool locally.

### Getting the sources

First, fork the GPSSample repository so that you can make a pull request. Then, clone your fork locally:

```
git clone https://github.com/<<<your-github-account>>>/gpssample.git
```

Occasionally you will want to merge changes in the upstream repository (the official code repo) with your fork.

```
git checkout main
git pull https://github.com/gpssample/gpssample.git main
```

Manage any merge conflicts, commit them, and then push them to your fork.

**Note**: The `gpssample/gpssample` repository contains a collection of GitHub Actions that help us with triaging issues. As you probably don't want these running on your fork, you can disable Actions for your fork via `https://github.com/<<Your Username>>/gpssample/settings/actions`.

### Build

### Where to Contribute
Check out the [full issues list](https://github.com/Microsoft/vscode/issues?utf8=%E2%9C%93&q=is%3Aopen+is%3Aissue) for a list of all potential areas for contributions. Note that just because an issue exists in the repository does not mean we will accept a contribution to the core editor for it. There are several reasons we may not accept a pull request like:

* Performance - One of Visual Studio Code's core values is to deliver a *lightweight* code editor, that means it should perform well in both real and perceived performance.
* User experience - Since we want to deliver a *lightweight* code editor, the UX should feel lightweight as well and not be cluttered. Most changes to the UI should go through the issue owner and/or the UX team.
* Architectural - The team and/or feature owner needs to agree with any architectural impact a change may make. Things like new extension APIs *must* be discussed with and agreed upon by the feature owner.

To improve the chances to get a pull request merged you should select an issue that is labelled with the [`help-wanted`](https://github.com/Microsoft/vscode/issues?q=is%3Aopen+is%3Aissue+label%3A%22help+wanted%22) or [`bug`](https://github.com/Microsoft/vscode/issues?q=is%3Aopen+is%3Aissue+label%3A%22bug%22) labels. If the issue you want to work on is not labelled with `help-wanted` or `bug`, you can start a conversation with the issue owner asking whether an external contribution will be considered.

To avoid multiple pull requests resolving the same issue, let others know you are working on it by saying so in a comment.

### Spell check errors

Pull requests that fix spell check errors in **translatable strings** (strings in `nls.localize(...)` calls) are welcomed but please make sure it doesn't touch multiple [feature areas](https://github.com/microsoft/vscode/wiki/Feature-Areas), otherwise it will be difficult to review. Pull requests only fixing spell check errors in source code are **not** recommended.

## Packaging

VS Code can be packaged for the following platforms: `win32-ia32 | win32-x64 | darwin-x64 | darwin-arm64 | linux-ia32 | linux-x64 | linux-arm`

These `gulp` tasks are available:

* `vscode-[platform]`: Builds a packaged version for `[platform]`.
* `vscode-[platform]-min`: Builds a packaged and minified version for `[platform]`.

👉 **Tip!** Run `gulp` via `npm` to avoid potential out of memory issues, for example `npm run gulp vscode-linux-x64`

See also: [Cross-Compiling for Debian-based Linux](https://github.com/Microsoft/vscode/wiki/Cross-Compiling-for-Debian-Based-Linux)

## Suggestions
We're also interested in your feedback for the future of VS Code. You can submit a suggestion or feature request through the issue tracker. To make this process more effective, we're asking that these include more information to help define them more clearly.

## Translations
We accept feedback on translations in language packs via GitHub issues in our [localization repo](https://github.com/Microsoft/vscode-loc/issues) that contains our currently supported language packs.

## Discussion Etiquette

In order to keep the conversation clear and transparent, please limit discussion to English and keep things on topic with the issue. Be considerate to others and try to be courteous and professional at all times.
