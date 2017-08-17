# Android Code Style @ GCX

## Installation on your local machine
1. Copy the [`AndroidTeam_latest.xml`](styles/AndroidTeam_latest.xml) into ``~/Library/Preferences/AndroidStudio{VERSION}/codestyles/``
2. Restart AndroidStudio
3. Select the codestyle scheme via `Preferences --> Editor --> Code Style`.
The codestyle will be enabled/used for **all projects** that are opened with AndroidStudio!

## Enabling project specific code styles for a project
If the codestyle is added to the git repository and IntelliJ is configured accordingly each project can have it's own style.

1. Install the [`AndroidTeam_latest.xml`](styles/AndroidTeam_latest.xml) locally (see above)
2. Restart AndroidStudio
3. In AndroidStudio, go to `Preferences --> Code style`
4. Open the scheme manager by clicking on `Manage...``
5. Select the code style and click `Copy to project`
6. In the scheme drop down select `Project`

Finally add the code style to the git repository:
```
git add -f .idea/codeStyleSettings.xml
```

## History
The currently latest version is always pointed to [`AndroidTeam_latest.xml`](styles/AndroidTeam_latest.xml).
This is always a copy of the styles with the highest version number.

A changelog can be found in the [CHANGELOG](CHANGELOG.md) file.

## Contributing
To contribute just change the codestyle locally to your needs.
Then you can create a PR to this repository.

The PR should always contain:
* Some information what have changed. Inside the [CHANGELOG.md](CHANGELOG.md).
* A updated [`AndroidTeam_latest.xml`](styles/AndroidTeam_latest.xml) to make it compareable to an older version.
* A new version in the [styles](/styles) folder.
