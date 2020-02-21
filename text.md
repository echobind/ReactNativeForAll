# Text Accessibility

Accessibly for text can be tricky and needs to be well thought within your application. Remember that with accessibility it can include how someone can actually see what we are displaying on the screen, or the use of a VoiceOver tool. We often use text of varying sizes and colors to represent information within our application.
Visual impairments can include low vision, color-blindness, and total blindness.

Do not use color of text alone to represent something of importance, like different status. Think red/yellow/green text to represent Error/warning/success. You should include other visual clues like an icon (but do not overuse those either).

Ensure that if the user has turned on accessibility text settings like large font size, that it does not render so poorly that it makes your app un-usable.

Use good contrasts and a readable font size

### Properties:
* **accessibleRole:**  'text' | 'header' | 'summary' | 'alert' | .... there are other potentials listed [here](https://facebook.github.io/react-native/docs/0.13/accessibility#accessibilityrole-ios-android)

* **accessibilityLabel:** string to be read by the screen reader when the user interacts with the image

* **accessible:** boolean, iOS only property that indicates whether or not the image is an accessibility element