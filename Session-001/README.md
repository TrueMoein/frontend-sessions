# Best Practices:

### 1. Folder structure

```
- shared-components
	- Table
		index.js
	- General
		- components
		    index.js
	-Sidebar
		- components
			SideBarItem.js
		    index.js
- views
	- Service1
		- components
		    index.js
	- Service2
		- components
		    index.js
```

### 2. Changelogs

current tools: auto-changelog => based on commit logs

New approach: https://keepachangelog.com/en/1.0.0/

feature branch => write changelogs into unreleased section

In case of deploying if deploy process is based on semver tags:

```
- update changelogs
	 - create a new released section and move all unreleased into this section
-git tag [tagName] => e.g. git tag v0.25.1-alpha
-git push --tags
```

For further detail checkout [here](https://github.com/semantic-release/semantic-release)
Follow commit conventions like [angular-commit-conventions](https://github.com/angular/angular.js/blob/master/DEVELOPERS.md#commits)