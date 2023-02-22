# godot-android-upload
Github Action to export a Godot game to the Google Play Store.  
If you are facing problems with the action or this README feels not complete, pull requests are welcome or open an issue.

## Table of contents
- [godot-android-upload](#godot-android-upload)
  - [Table of contents](#table-of-contents)
  - [Requirements](#requirements)
  - [Parameters](#parameters)
  - [Working examples](#working-examples)
  - [License](#license)

## Requirements
 - Google Play Store Developer Account
 - Google Service Account JSON file
 - Godot Project with a Android Export

## Parameters
| key | required | default | description |
| ----|----------|---------|-------------|
| package-name | true |   | Android package name |
| release-file | true |   | Path to the .apk or .aab file |
| release-track | false | internal  | Release track: production, beta, alpha, internalsharing, internal |
| changes-not-sent-for-review | false | false | Indicates that the changes in this edit will not be reviewed until they are explicitly sent for review from the Google Play Console |
| working-directory | false | . | Path to .project file |
| service-account-json | false | service-account.json | Path tho your Google service-account.json file  |
| godot-version | false | 3.5 | Check versions [here](https://downloads.tuxfamily.org/godotengine/) |
| cache-version | false | 1 | Headless godot gets cached, on problems increase version |

## Working examples
You an find a working examples here:  
https://github.com/dulvui/pocket-broomball/blob/main/.github/workflows/upload-android.yml

## License
This software is licensed under the [MIT license](LICENSE).