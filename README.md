# godot-android-export
Github Action to export a Godot game for Android to apk/aab.  
If you are facing problems with the action or this README feels not complete, pull requests are welcome or open an issue.

## Table of contents
- [godot-android-export](#godot-android-export)
  - [Table of contents](#table-of-contents)
  - [Requirements](#requirements)
  - [Parameters](#parameters)
  - [Working examples](#working-examples)
  - [Version 2 breaking changes](#version-2-breaking-changes)
  - [License](#license)

## Requirements
 - Godot Project
 - A valid exports_preset.cfg with an Android config

## Parameters
| key | required | default | description |
| ----|----------|---------|-------------|
| godot-version | true | . | Godot Engine version. Supported are 4.x versions. Check versions [here](https://github.com/godotengine/godot-builds/releases) |
| godot-channel | false | stable | Godot Engine release channel (stable, beta, rc1, rc2, rc3...). Defaults to 'stable' Check release channels [here](https://github.com/godotengine/godot-builds/releases) |
| working-directory | false | . | Path to project.godot file |

## Working examples
You an find a working examples here:  
https://github.com/dulvui/pocket-broomball/blob/main/.github/workflows/upload-android.yml
https://github.com/dulvui/ball2box/blob/main/.github/workflows/upload-android.yml

## Version 2 breaking changes
The repository and action has been renamed from godot-android-upload to simply godot-android-export to simplify the action and to remove third party actions dependencies.
Now this actions follows the Unix philosophy of simply doing one thing well.
You can then upload the aab/apk export  of your game where ever you want.

## License
This software is licensed under the [MIT license](LICENSE).
