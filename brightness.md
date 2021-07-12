This shortcut is a case study on how to dynamically set brightness based on a calculation on the current brightness level.
I use it as home automation.

#Dependencies
- Apple Shortcuts: https://support.apple.com/guide/shortcuts/welcome/ios
- "Magic variables" concept: https://support.apple.com/guide/shortcuts/use-variables-apdd02c2780c/4.0/ios/14.0
#When:
- set to: battery level falls below (your desired value)

#Do
All elements are found in the "Scripting" section.
a. Device, "Get Device Details", then select "Current Brightness"
b. Math, "Calculate"
  b.1. Select "Current Brightness" as first number, 
  b.2. Select operand "divide", 
  b.3. Input the desired divider number (e.g. 2)
c. Math, "Round"
  c.1. Select "Calculation Results"
  c.2. Select to "Tenths"
d. Device, "Set Brightness" to "Rounded Number" (long press the default value)

