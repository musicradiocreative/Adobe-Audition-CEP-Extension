# Adobe Audition CEP Extension for Music Radio Creative

A Music Radio Creative powered panel that can be docked inside Adobe Audition CC.

### Installation

#### macOS

* Move the contents of the *download* folder from this repo to ~/Library/Application Support/Adobe/CEP/extensions/ on your local computer.
* This app will not currently run unless Adobe apps are switched to developer mode. Do this by typing this command into Terminal:
`defaults write com.adobe.CSXS.8 PlayerDebugMode 1`
* Launch Adobe Audition CC and click Window > Extensions > Music Radio Creative.

### Development

* The app will call a website inside the panel which can be docked, resized, opened and closed.
* It's a Chromium embeded browser in a panel which should play video, sounds and more.
* Anything that would work with standard HTML5 should work here (embeds, localStorage, cookies etc.)

#### Core Files

*index.html* - just does a javascript redirect to musicradiocreative.com. Any custom logic can exist on the server in this case, and be easily updateable.

*manifest.xml* - describes the name, identifier, version, and some panel information.

### Resources

[Adobe CEP on GitHub](https://github.com/Adobe-CEP) - Official samples and resources from the Adobe CEP team.
[Script Loader for Adobe Audition](https://github.com/Adobe-CEP) - Handy tool for loading JSX scripts in Adobe Audition.
[Notes Panel for Adobe Audition](https://github.com/Hennamann/Notes-Panel-for-Adobe-Audition) - Awesome Notes Plugin for Adobe Audition from [Ole Henrik Stabell](https://github.com/Hennamann).