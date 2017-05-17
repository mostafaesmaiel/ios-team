Welcome
============

The home of iOS conichi team.

## Fresh Start

If you're a new developer in a team start with the following:

```sh
git clone https://github.com/conichiGMBH/ios-team-guidelines.git
cd ios-team-guidelines
scripts/bootstrap_ruby.sh
```

and after ruby is installed correctly execute script to clone and bootstrap all repos

```sh
scripts/bootstrap_projects.sh
```

## Guides

These guides are not to blindly followed but to discuss when in doubt.

* [Swift Style Guide](https://github.com/conichiGMBH/ios-team/blob/master/docs/swift_style_guide.md)
* [Objective-C Style Guide](https://github.com/conichiGMBH/ios-team/blob/master/docs/objective_c_style_guide.md)
* [Code Review Guide](https://github.com/thoughtbot/guides/tree/master/code-review)
* [Git Guide](https://github.com/conichiGMBH/ios-team/blob/master/docs/git_protocol.md)
* [PR Guide](https://github.com/conichiGMBH/ios-team/blob/master/docs/pr_protocol.md)
* [Accesibility Naming Guide](https://github.com/conichiGMBH/ios-team/blob/CNI-5559/docs/accessibility_naming_guide.md)
* [New Project Guide](https://github.com/conichiGMBH/ios-team/blob/master/docs/new_project_guide.md)
* [CI Guide](https://github.com/conichiGMBH/ios-team/blob/master/docs/ci_guide.md)
* [Things to Remember in First Day](https://github.com/conichiGMBH/ios-team/blob/CNI-5939/docs/things_to_remember.md)

## Technology Stack

* Objective-C - most of the codebase is written in Objective-C, but new features are considered to be written in Swift.
* Swift - some apps have been already migrated to support Swift language, but if not ready yet, create a respective task and do so 🚀
* [CocoaPods](https://github.com/CocoaPods/CocoaPods) - as a main dependency manager, we use CocoaPods, but for the OSS project don't forget about [Carthage](https://github.com/Carthage/Carthage) and [Swift Package Manager](https://github.com/apple/swift-package-manager) if available.
* Bundler - we use `Gemfile` to manage our `ruby` dependencies. Recommend to read [Gemfile Guide](https://guides.cocoapods.org/using/a-gemfile.html).

## Testing

We do test all our apps to ensure that our behavior is what we expect. Initially the codebase was written by `XCTest` framework. Recently we migrated to [Quick](https://github.com/Quick/Quick/) and [Specta](https://github.com/specta/specta).

For the UI tests we use extensively [FBSnapshotTests](https://www.objc.io/issues/15-testing/snapshot-testing/). We use iOS 9.3 as a main version for all UITests and all screenshots are captured in iPhone 6, iPhone 6 Plus, iPhone 5s and iPad Air simulators.
