# CoFrance Config Files

This repository provides CoFrance Config Files with automatic download during the plugin initialisation. <br>


## How to contribute
- Fork this repository.
- Check [wiki](https://github.com/AlexisBalzano/CoFrance-Config-Files/wiki) to understand the layout and properties of each file.
- Update files (if using a code editor, the schema should highlight any error) without modifying `"version"` property.
- Push your changes to Github, Github should run and validate all files using Actions:
  - if validation fails, fix errors printed inside the Action report
  - if validation succeeds, it will automatically update all modified files version and `version.json` file.
- Create a pPull Request on main branch of this repository for review.

## How version checking works
During initialisation, the plugin will fetch `version.json` file and compare local file version with the ones provided inside this file. <br>
If a newer version is available, and plugin version matches, the plugin will download corresponding config file.
<br>
If `version.json` define a different version for one file that the `"version"` property states inside that file, it will force the redownload of said file during every CoFrance Initialisation. <br>
To avoid such a case, check that those matche when creating the Pull Request.
