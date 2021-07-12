This shortcut is a case study on dynamically setting brightness based on calculating the current brightness level.
I use it as home automation.

# Dependencies
- Apple Shortcuts: https://support.apple.com/guide/shortcuts/welcome/ios
- "Magic variables" concept: https://support.apple.com/guide/shortcuts/use-variables-apdd02c2780c/4.0/ios/14.0
# When:
- set to: battery level falls below (your desired value)

# Do
In the "Scripting" section, you can find all the required elements.
- Device, "Get Device Details", then select "Current Brightness"
- Math, "Calculate"
  - Select "Current Brightness" as the first number, 
  - Select operand "divide", 
  - Input the desired divider number (e.g. 2)
- Math, "Round"
  - Select "Calculation Results"
  - Select to "Tenths"
- Device, "Set Brightness" to "Rounded Number" (long-press the default value)

![Screenshot](https://user-images.githubusercontent.com/5004428/125288259-37d28680-e31e-11eb-82d2-85f73421dde9.jpeg)
