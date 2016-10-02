# SKTRings
Animated ring charts in SpriteKit for watchOS 3. Supports bounce easing and color change effects.

The Activity app is one of the prominent features of the Apple Watch. Imagine if the Activity app’s rings could animate to their current value with a bounce effect or change color depending on how recently you moved. Those animations would be both magical and useful. However, you’d have a hard time implementing them with a sequence of images like you used in watchOS 2. Instead, now you can use SpriteKit to achieve those animations.

`SKRingNode` performs the bulk of the calculations and drawing of the ring so that you can focus on the animations you’ll add to it. `SKNestedRingNode` simplifies creating multiple concentric rings.

SKTRings relies on SKTUtils, an open source project published by the raywenderlich.com team. You can check it out on GitHub at [bit.ly/2dcyDyz](http://bit.ly/2dcyDyz).

There’s only one file inside SKTUtils that’s not shared with the WatchKit Extension, SKTAudio.swift. Its code refers to `AVFoundation` which is not available in watchOS.
