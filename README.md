# CoFrance v2
The next evolution of French ATC Solutions.

## Screenshots
<p align="center">
<img width="49%" height="49%" alt="CoFrance Agenda Preview" src="https://github.com/user-attachments/assets/6f45253e-1e9c-4fc4-8c36-2b223ac6aebc" />
<img width="49%" height="49%" alt="CoFrance LFBB Preview" src="https://github.com/user-attachments/assets/68ec52ed-688c-4446-bd4d-e9ea42519933" />
</p>
<p align="center">
<img width="49%" height="49%" alt="CoFrance CDG Preview" src="https://github.com/user-attachments/assets/e33e259b-60d9-4816-a79f-b17814b1565b" />
<img width="49%" height="49%" alt="CoFrance TRANS Popup Preview" src="https://github.com/user-attachments/assets/5cd3f288-0450-42fb-bfe5-54da9c4470c6" />
</p>
<p align="center">
<img width="49%" height="49%" alt="CoFrance LFEE Preview" src="https://github.com/user-attachments/assets/6432bc52-cd05-429b-b18f-8dff105b9137" />
<img width="49%" height="49%" alt="CoFrance List Preview" src="https://github.com/user-attachments/assets/9c2f15ef-a7b5-4168-a1e8-af27e86e0f2b" />
</p>

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
During initialisation, the plugin will fetch `version.json` file and compare local `version.json` file versions with the ones provided inside this file. <br>
If a newer version is available the plugin loader will download corresponding config file.
<br>
