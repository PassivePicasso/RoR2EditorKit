# RoR2EditorKit - Editor Utilities, Inspectors and More for Risk of Rain2

## About

RoR2EditorKit is a *Thunderkit Extension* for developing mods inside the UnityEditor, providing a myriad of Inspectors, Property Drawers, Editor Windows and more.

At it's core, RoR2EditorKit should not have any classes or systems that depend on runtime usage, RoR2EditorKit works exclusively for speeding up the modding enviroment.

## Manual Installation

To download *RoR2EditorKit* to your thunderkit project you'll need thunderkit version 3.4.0 or greater in your project.

* 1.- Open the ThunderkitSettings window (Tools/Thunderkit/Settings) and look at the PackageSourceSettings.
* 2.- If a PackageSource that points to https://thunderkit.thunderstore.io exists, skip to step 6, otherwise, continue
* 3.- Click the Add button, and on the dropdown menu, select ThunderstoreSource
* 4.- Select the new ThunderstoreSource, name "Package Source:" to "Thunderkit Extensions" and "Url:" to https://thunderkit.thunderstore.io
* 5.- Close ThunderkitSettings, open the Packages window (Tools/Thunderkit/Packages).
* 6.- Expand the Thunderkit Extensions menu, select RoR2EditorKit. Hit Install.
* 7.- You've now installed RoR2EditorKit to your project.

Once installed, it is heavily reccommended to open the ThunderkitSettings window to modify certain settings that RoR2EditorKit will use while helping you develop the mod.

* RoR2EditorKitSettings: Settings of the extension itself
 * Token Prefix: A prefix for your mod, it's used to generate unique tokens.
 * Main Manifest: The manifest of your mod, used in a myriad of tools to know the assetbundle or the main DLL.

## Extending RoR2EditorKit's Functionality.

* In case you need to extend RoR2EditorKit's functionality for your own purposes (Such as a custom inspector for a mod you're working on), you can look into this wiki page that explains how to extend the editor's functionality using RoR2EditorKit's systems.

[link](https://github.com/risk-of-thunder/RoR2EditorKit/wiki/Extending-the-Editor's-Functionality-with-RoR2EditorKit's-Systems.)

## Contributing

Contributing to RoR2EditorKit is as simple as creating a fork, and cloning the project. the main folder (RoR2EditorKit) is a unity project itself. Simply opening it with the unity version ror2 uses will allow you to edit the project to your heart's content.

A more detailed Contribution guideline can be found [here](https://github.com/risk-of-thunder/RoR2EditorKit/blob/main/CONTRIBUTING.md)

## Changelog

(Old changelogs can be found [here](https://github.com/risk-of-thunder/RoR2EditorKit/blob/main/RoR2EditorKit/Assets/RoR2EditorKit/OldChangelogs.md))

### Current

### 1.0.0

* First Risk of Thunder release
* Rewrote readme a bit
* Added missing XML documentation to methods
* Added a property drawer for PrefabReference (Used on anything that uses RendererInfos)
* Added the MaterialEditor
    * The material editor is used for making modifying and working with HG shaders easier.
    * Works with both stubbed and non stubbed shaders
    * Entire system can be disabled on settings
* Properly added an Extended Property Drawer
* Added Inspector for CharacterBody
* Added Inspector for Child Locator
* Added Inspector for Object Scale Curve
* Added Inspector for BuffDef
* Fixed the enum mask drawer not working with uint based enum flags
