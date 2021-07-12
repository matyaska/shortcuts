This shortcut is a case study on dynamically setting brightness based on calculating the current brightness level.
I use it as home automation.

#Dependencies
- Apple Shortcuts: https://support.apple.com/guide/shortcuts/welcome/ios
- "Magic variables" concept: https://support.apple.com/guide/shortcuts/use-variables-apdd02c2780c/4.0/ios/14.0
#When:
- set to: battery level falls below (your desired value)

#Do
In the "Scripting" section, you can find all the required elements.
a. Device, "Get Device Details", then select "Current Brightness"
b. Math, "Calculate"
  b.1. Select "Current Brightness" as the first number, 
  b.2. Select operand "divide", 
  b.3. Input the desired divider number (e.g. 2)
c. Math, "Round"
  c.1. Select "Calculation Results"
  c.2. Select to "Tenths"
d. Device, "Set Brightness" to "Rounded Number" (long-press the default value)

![Screenshot](https://user-images.githubusercontent.com/5004428/125288259-37d28680-e31e-11eb-82d2-85f73421dde9.jpeg)
