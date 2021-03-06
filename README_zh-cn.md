# Flutter Cupertino Date Picker

[[Pub Packages]](https://pub.dartlang.org/packages/flutter_cupertino_date_picker)

Flutter 的日期选择器控件，iOS 样式。

![示例](http://openproject.oss-cn-beijing.aliyuncs.com/images/flutter/date_picker1.png!image_scale1)

## 用法

#### 1\. 添加依赖

在项目的 `pubspec.yaml` 文件中添加依赖：

```yaml
dependencies:
  flutter_cupertino_date_picker: ^0.0.3
```

#### 2\. 获取包

执行 Flutter 的命令获取包资源：

```bash
$ flutter packages get
```

#### 3\. 导入控件

在项目中导入该控件：

```dart
import 'packages:flutter_cupertino_date_picker/flutter_cupertino_date_picker.dart';
```

#### 4\. 显示控件

```dart
///
/// context: BuildContext.
/// showTitleActions: 是否显示带有确定、取消按钮的标题栏。
/// minYear: 年份选择器的最小值，默认值：1900年。
/// maxYear: 年份选择器的最大值，默认值：2100年。
/// initialYear: 年份选择器的初始值。
/// initialMonth: 月份选择器的初始值。
/// initialDate: 日期选择器的初始值。
/// onChange: 当前选择的日期改变时的回调事件。
/// onConfirm: 点击标题栏确定按钮的回调事件。
DatePicker.showDatePicker(
  context,
  showTitleActions: true,
  minYear: 1970,
  maxYear: 2020,
  initialYear: 2018,
  initialMonth: 6,
  initialDate: 21,
  onChanged: (year, month, date) { },
  onConfirm: (year, month, date) { },
);
```

***showTitleActions: false***

![示例: showTitleActions=false](http://openproject.oss-cn-beijing.aliyuncs.com/images/flutter/date_picker2.png!image_scale1)

## 示例

[示例源码](https://github.com/wuzhendev/flutter-cupertino-date-picker/tree/master/example)

## Futures

1. 对显示的日期进行格式化处理。
2. 国际化。

## License

```
Copyright 2018 wuzhen

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
