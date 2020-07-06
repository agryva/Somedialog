# Somedialog
[![pub package](https://img.shields.io/pub/v/somedialog.svg)](https://pub.dev/packages/somedialog#-readme-tab-)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
[![support](https://img.shields.io/badge/platform-flutter%7Cflutter%20web-ff69b4.svg?style=flat-square)](https://github.com/agryva/Somedialog)

Flutter package for handle a nice dialog ui

## Help Maintenance
I've taken the time to make this library, help support to develop it or buy me coffee and snacks to be even more enthusiastic
<br/>
<a href="https://www.buymeacoffee.com/agryva" target="_blank"><img src="https://www.buymeacoffee.com/assets/img/custom_images/purple_img.png" alt="Buy Me A Coffee" style="height: auto !important;width: auto !important;" ></a>
[![Paypal](https://www.paypalobjects.com/webstatic/mktg/Logo/pp-logo-100px.png)](https://paypal.me/agryva)

| <img src="https://raw.githubusercontent.com/agryva/Somedialog/master/screen/dialog.jpg" width="379px;"/><br /><sub><b>Dialog</b></sub>  |
| :---: |

## Getting Started

### Setup
Add dependency to your pubspec.yaml:

```dart
somedialog: ^{latest_version}
```


### Basic use
First, add an import to your code:
```dart
import 'package:somedialog/somedialog.dart';

FlatButton(
              child: Text("Show Dialog"),
              onPressed: () {
                SomeDialog(
                  context: context,
                  path: "assets/report.json",
                  mode: SomeMode.Lottie,
                  content:
                      "Please before tracking, double-check the code you entered!",
                  title: "Are you sure ?",
                  submit: () {
                  }
                );
              },
            )
```

## SomeMode
| SomeMode |
| :---------------------- |
| Lottie
| Network
| Asset


## Parameters
| parameter                   | types           | defaultValues                                                                                                     |
| :---------------------- | :-------------: | :---------------------------------------------------------------------------------------------------------------: |
| buttonConfig        | `buttonConfig`        | ButtonConfig() |
| path        | `string`        |  |
| title        | `string`        |  |
| content        | `string`        |  |
| dialogHeight        | `double`        | 310 |
| imageHeight        | `double`        | 150 |
| imageWidth        | `double`        | 150 |
| submit        | `Function`        |  |
| mode| `SomeMode`     |  |