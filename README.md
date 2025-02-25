## Mask guide implemented with ColorFilter, refer by [https://juejin.cn/post/7089087097218269197](https://juejin.cn/post/7089087097218269197)

## Getting started

```dart
import 'package:mask_guide/mask_guide.dart';
```

## Usage

### First of all, add `MaskGuideNavigatorObserver()` in `MaterialApp()`

```
MaterialApp(
 navigatorObservers: [MaskGuideNavigatorObserver()],
)
```

### Usage of Custom Step Widget

Extend the `StepWidget` and override `preStep`, `nextStep`, `doneCallBack` if you need.

To create a custom step widget, you should calculate the position of the widget yourself.

```
class CustomStepWidget extends StepWidget

@override
void preStep() {
 super.preStep();
 // todo: do something
}

@override
void nextStep() {
 super.nextStep();
 // todo: do something
}

@override
void doneCallBack() {
 super.doneCallBack();
 // todo: do something
}
```
Check [example](https://github.com/Dabbit-Chan/mask_guide/tree/master/example) for more.
