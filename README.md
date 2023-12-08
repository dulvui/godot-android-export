# godot-android-export
Github Action to export a Godot Engine 3 and 4 game for Android to apk/aab.  
If you are facing problems with the action or this README feels not complete, pull requests are welcome or open an issue.

## Table of contents
- [godot-android-export](#godot-android-export)
  - [Table of contents](#table-of-contents)
  - [Godot 4.x support](#godot-4x-support)
  - [Requirements](#requirements)
  - [Parameters](#parameters)
  - [Working examples](#working-examples)
  - [Version 2 breaking changes](#version-2-breaking-changes)
  - [License](#license)

## Godot 4.x support
I start now to adapt the action for Godot 4.  
Godot 3 will be available under the v3.x.x tag and Godot 4 under 4.x.x tag

## Requirements
 - Godot Project
 - A valid exports_preset.cfg with an Android config

## Parameters
| key | required | default | description |
| ----|----------|---------|-------------|
| working-directory | false | . | Path to project.godot file |
| godot-version | false | 3.5.3 | Check versions [here](https://downloads.tuxfamily.org/godotengine/) |

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