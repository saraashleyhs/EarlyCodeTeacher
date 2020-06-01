##### [Additional Information]
When using percentages as values it's important to include the `min-width/height` and `max-width/height` properties so as to avoid your elements being rendered in sizes that are unmanageable for the user. See below:

```css
body {
  width: auto;
  height: auto;
  min-width: 100pt;
  max-width: 1000pt;
  min-height: 150pt;
  max-height: 1500pt;
}
```