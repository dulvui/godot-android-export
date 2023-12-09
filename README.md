# godot-android-export
Github Action to export a Godot Engine 3 and 4 game for Android to apk/aab.  
If you are facing problems with the action or this README feels not complete, pull requests are welcome or open an issue.

## Table of contents
- [godot-android-export](#godot-android-export)
  - [Table of contents](#table-of-contents)
- [Godot 4.x](#godot-4x)
  - [Requirements](#requirements)
  - [Parameters](#parameters)
  - [How to use](#how-to-use)
  - [Working examples](#working-examples)
- [Godot 3.x](#godot-3x)
  - [Requirements](#requirements-1)
  - [Parameters](#parameters-1)
  - [How to use](#how-to-use-1)
  - [Working examples](#working-examples-1)
  - [Version 2 breaking changes](#version-2-breaking-changes)
  - [License](#license)

# Godot 4.x
Godot 4.x is the current active stable version and will be actively maintained.
You can find the code in the `main` branch.

## Requirements
 - Godot Project
 - A valid exports_preset.cfg with an Android config
 - A valid export_credentials.cfg

## Parameters
| key | required | default | description |
| ----|----------|---------|-------------|
| working-directory | false | . | Path to project.godot file |
| godot-version | false | 4.x | Check versions [here](https://downloads.tuxfamily.org/godotengine/) |

## How to use
Use the 4.x tag
```
- name: Godot Android export
  uses: dulvui/godot-android-export@v4.0.0
  with:
    working-directory: game
    godot-version: 4.2
```

## Working examples
You an find a working examples here:  
https://github.com/dulvui/futsal-manager/blob/main/.github/workflows/upload-android.yml

# Godot 3.x
Godot 3.x is the current LTS version and will be less actively maintained.
You can find the code in the `godot-3` branch.

## Requirements
 - Godot Project
 - A valid exports_preset.cfg with an Android config

## Parameters
| key | required | default | description |
| ----|----------|---------|-------------|
| working-directory | false | . | Path to project.godot file |
| godot-version | false | 3.x | Check versions [here](https://downloads.tuxfamily.org/godotengine/) |

## How to use
Use the 3.x tag
```
- name: Godot Android export
  uses: dulvui/godot-android-export@v3.0.0
  with:
    working-directory: game
    godot-version: 3.5.3
```

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