[download]: https://github.com/diogo-webber/vox-launcher/releases/latest/download/VoxLauncher.zip
[download_count]: https://img.shields.io/github/downloads/diogo-webber/vox-launcher/total?style=for-the-badge&labelColor=%232d333b&color=%23066094
[version]: https://img.shields.io/github/v/release/diogo-webber/vox-launcher?style=for-the-badge&labelColor=%232d333b&color=%23066094
[python_version]: https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&labelColor=%232d333b&color=%23066094
[video_tutorial]: https://youtu.be/dxl-RV0LtEA
[locales]: https://ss64.com/locale.html
[pull_request]: https://github.com/diogo-webber/vox-launcher/compare/
[new_issue]: https://github.com/diogo-webber/vox-launcher/issues/new
[token_website]: https://accounts.klei.com/account/game/servers?game=DontStarveTogether
[pyinstaller_repo]: https://github.com/pyinstaller/pyinstaller
[windows_defender_tutorial]: https://support.microsoft.com/en-us/windows/add-an-exclusion-to-windows-security-811816c0-4dfd-af4a-47e4-c301afe13b26

<h1 align="center">

  ![GitHub Release][version]
  &ensp;
  ![GitHub Downloads][download_count]
  &ensp;
  ![Python Version)][python_version]

</h1>

<br>

<img src="/app/assets/icon.ico" align="left" width="185px"/>

### Vox Launcher

> A Don't Starve Together dedicated server launcher.

<br><br><br><br><br>

`Vox Launcher` is a Windows only dedicated server launcher, created with the aim of simplifying their creation and usage.

<br>

### Included features:
- Buttons to **save**, **reset**, **rollback** and **stop** the server.
- A screen that shows server logs and have a console for executing commands.
- Shows information about the server, such as **number of players**, **day count**, **season** and **memory usage**.
- Supports any number of shards.

<br>

## How it works?

<br>

- Download the `App` zip, extract its contexts and start the `Vox Launcher` executable. [**Click here**][download] to download it.
- Select the game installation folder under `Game Directory`, if it has not been automatically populated.
- Create a world using the in game menu and select it under `Cluster Directory`.
- Paste a server token under `Server Token`. See instructions on how to obtain one in the app.
- Finally, click on the `LAUNCH` button and have fun!

<br>

<dl><dd><dl>
  
> [!TIP]
> Additionally, check out this amazing **[video tutorial][video_tutorial]** by Jazzy Games on YouTube.

</dl></dd></dl>

<br>

## Frequently Asked Questions

<br>

- **Windows Defender is flagging Vox Launcher as a threat, why is this happening?**

<dl><dd><dl><dd><dl>
 
> The tool called [**Pyinstaller**][pyinstaller_repo], which is used to bundle the app into an executable, is also used by people who actually make malicious software. Windows Defender recognizes some similar patterns in the executable and includes Vox Launcher as a threat.

> Usually creating a new version solves this temporarily, but there's not much to be done in the long term other than rebuilding the whole app in another programming language, which I don't have the time or desire to do at the moment. The only thing you could do is to [**add an exclusion to Windows Defender**][windows_defender_tutorial].

</dl></dd></dl></dd></dl>

<br>

- **Are mods supported? What do I need to do to enable them?**

<dl><dd><dl><dd><dl>
 
> Yes, they are. Just enable them when you're creating the world, it's that simple!

</dl></dd></dl></dd></dl>

<br>

- **How do I get a Cluster Token?**

<dl><dd><dl><dd><dl>
 
> You can create one on the [**Klei Accounts**][token_website] website.

</dl></dd></dl></dd></dl>

<br>

- **I've found a problem in the app, where should I report it?**

<dl><dd><dl><dd><dl>
 
> You may create a issue in the [**Issues Tab**][new_issue].</br>Please attach the app log file when doing so. It can be found at `appdata/logs/applog.txt`.

</dl></dd></dl></dd></dl>

<br>

## App Showcase

<br>

From top left to bottom right: `Instructions`, `Starting Server`, `Server Online`, `Log Screen`.

<br>

<div align="center">

<img align="left" src="/github_assets/offline.png" width=45%/>
<img align="left" src="/github_assets/starting.png" width=45%/>

</div>

<br><br><br><br><br><br><br><br><br><br><br><br><br>

<div align="center">

<img align="left" src="/github_assets/online.png" width=45%/>
<img align="left" src="/github_assets/logscreen.png" width=45%/>

</div>


<br><br><br><br><br><br><br><br><br><br><br><br><br><br>

## 📌 Contributing

<br>

Feel free to suggest features and create pull requests to fix bugs or improve existing code. The entry point is `app/main.py`.

#### You can also help by translating the app:
- Create a file in `app/localization/` called `locale.yaml`, where locate is the language code, which you can find in **[this website][locales]**.
  
- Use `en_US.yaml` as a template. Please, try to keep sentence lengths close to the English version to avoid visual issues.
  
- Create a **[Pull Request][pull_request]** with the title: `Added {language} ({lang_code}) localization`

<br>

#### Installing dependencies:
```ruby
  python -m pip install -r requirements.txt
```

<br><br>

## 📜 License

<br>

This project is under MIT license. See the [**LICENSE**](LICENSE) file for more details.
