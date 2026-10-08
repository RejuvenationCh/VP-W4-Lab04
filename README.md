# lab04

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Learn Flutter](https://docs.flutter.dev/get-started/learn-flutter)
- [Write your first Flutter app](https://docs.flutter.dev/get-started/codelab)
- [Flutter learning resources](https://docs.flutter.dev/reference/learning-resources)

For help getting started with Flutter development, view the
[online documentation](https://docs.flutter.dev/), which offers tutorials,
samples, guidance on mobile development, and a full API reference.
# VP-W4-Lab04

## Check yourself

1. **A `Text` inside a `Row` overflows. Which layout rule was broken?** The `Row` gave the non-flexible `Text` no useful width limit, so the text chose its natural size and the children together exceeded the width from the parent. This breaks the relationship between constraints going down and sizes going up.

2. **Why is `width: 150` the wrong fix?** It only fits one screen and text size. A narrower screen, longer name, or wider test font can overflow again.

3. **Why not use `SingleChildScrollView` with `shrinkWrap: true` on the list?** The 500 items test fails because the list can measure and build far more items than are visible. That becomes slow and memory heavy when an API returns a large menu.

4. **Why use `LayoutBuilder` for the tablet layout?** It measures the space actually available to the menu. `MediaQuery.sizeOf(context)` reports the device size, which might not match the space given to this part of the screen.

5. **Why does the empty data crash belong in a layout lab?** The screen tried to read promo items that did not exist, so it could not render. A responsive screen also needs a usable layout when there is no data.
