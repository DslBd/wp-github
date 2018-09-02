WP Github
=========

Display users public Github profile, repositories, commits and issues.

## Usage

You can install the widgets in your sidebars from the widgets section in wordpress once the plugin ins installed and enabled.

You also can use shortcodes to display github content on your posts and pages.

## Shortcodes

Admin option will let you add a default usernamme and repository so you don't have to add it in the shortcode eachtime.

#### Profile
```html
[github-profile]
```
Argument | Example | Description
--- | --- | ---
username | `[github-profile username="armandsl"]` | Displays the profile box for the user seinoxygen.

#### Repository clone urls
```html
[github-clone]
```
Argument | Example | Description
--- | --- | ---
username | `[github-clone username="armandsl"]` | Show ssh & https url.
limit | `[github-clone username="armandsl" repository="wp-github"]` | From a selected repo.

#### Repositories
```html
[github-repos]
```
Argument | Example | Description
--- | --- | ---
username | `[github-repos username="armandsl"]` | Lists up to 5 repositories from the user armandsl.
limit | `[github-repos username="armandsl" limit="10"]` | Lists up to 10 repositories from the user armandsl.

#### Commits
```html
[github-commits]
```
Argument | Example | Description
--- | --- | ---
username | `[github-commits username="armandsl"]` | main username
repository | `[github-commits username="armandsl" repository="wp-github"]` | Lists up to 5 commits from the repository wp-github.
limit | `[github-commits username="armandsl" repository="wp-github" limit="10"]` | Lists up to 10 commits.
xtended | [github-commits username="armandsl" repository="wp-github" limit="30" xtended='{"Date de commit": "commit:committer:date","Email committer": "commit:committer:email","Url de commit": "url"}'] | allow to get custom data, Caution XPERIMENTAL! json format, rely on github api endpoints

For correct listing username and repository **_are_** required.

#### Issues
```html
[github-issues]
```
Argument | Example | Description
--- | --- | ---
username | `[github-issues username="armandsl"]` | main username
repository | `[github-issues username="armandsl" repository="wp-github"]` | Lists up to 5 issues from the repository wp-github.
limit | `[github-issues username="armandsl" repository="wp-github" limit="10"]` | Lists up to 10 issues from the repository wp-github.


#### Issue
```html
[github-issue]
```
Argument | Example | Description
--- | --- | ---
username | `[github-issue username="armandsl"]` | main username
repository | `[github-issue username="armandsl" repository="wp-github"]` | selected repo
number | `[github-issue username="armandsl" repository="wp-github" number="14"]` | issue number

#### Pull request
```html
[github-pulls]
```
Argument | Example | Description
--- | --- | ---
username | `[github-pulls username="armandsl"]` | main username
repository | `[github-pulls username="armandsl" repository="wp-github"]` | from the repository wp-github.
limit | `[github-pulls username="armandsl" repository="wp-github" limit="10"]` | Lists up to 10 pull request from the repository wp-github.

#### Gists
```html
[github-gists]
```
Argument | Example | Description
--- | --- | ---
username | `[github-gists username="armandsl"]` | Lists up to 5 gists from the user armandsl.
limit | `[github-gists username="armandsl" limit="10"]` | Lists up to 10 gists from the user armandsl.

#### File content
```html
[github-contents]
```
Argument | Example | Description
--- | --- | ---
username | `[github-contents username="armandsl"]` |Add username (except if filled in wp BO.
repository | `[github-contents username="armandsl" repository="wp-github"]` | pick up a repository from the user armandsl.
filepath | `[github-contents username="armandsl" repository="wp-github" filepath="wp-github.css"]` | Select a file with full path in the repository.
language | `[github-contents username="armandsl" repository="wp-github" filepath="wp-github.css" language="css"]` | Help JsHighlighter if exists, will generate code inside PRE and CODE tags.

#### Releases
```html
[github-releases]
```
Argument | Example | Description
--- | --- | ---
username | `[github-releases username="armandsl"]` |Add username (except if filled in wp BO.
repository | `[github-releases username="armandsl" repository="wp-github"]` | pick up a repository from the user armandsl.
limit | `[github-releases username="armandsl" repository="wp-github" limit="10"]` | Lists up to 10 releases.
 
#### Latest release
 ```html
 [github-releaseslatest ]
 ```
 Argument | Example | Description
 --- | --- | ---
 username | `[github-releaseslatest username="armandsl"]` |Add username (except if filled in wp BO.
 repository | `[github-releaseslatest username="armandsl" repository="wp-github"]` | pick up a repository from the user armandsl.
