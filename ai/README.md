# Understanding the JSON files for AI

### Across All files

Variable Name | Type | Description
----------------------------------
ButtonText | String | the text that appears on the command button in the AI interface
selectSpeech | Array | a series of variables that affect the text that appears appear when the command is selected
successSpeech | Array | same as above, but appears after the command has been issued and executed successfully
failSpeech | Array | as above; appears after a command has been issued but did not execute
animation | String | animation to play as text scrolls, options are **talk** / **yell** / **refuse** / **unique**
text | String | Dialogue of the AI for the associated speech
speedModifier | Floating point | Multiplier for how fast the associated speech scrolls

### In ai.config.patch

Variable Name | Type | Description
----------------------------------
aiFrames | String | path to a file of the AI's image
portraitFrames | String | path to a file of the AI's image for use in missions
staticFrames | String | path to an image file of static; overlayed on the AI's image
openSpeech | Array | series of variables that affect the text that appears when you open the AI interface
openSpeech/0 | Array | initial opening dialogue for AI
openSpeech/1 | Array | opening dialogue after you've rebooted the AI but before unlocking inter-system travel
openSpeech/2 | Array | opening dialogue after unlocking inter-system travel but before unlocking FTL travel
openSpeech/3 | Array | opening dialogue after unlocking FTL travel
techIntro | Array | dialogue for opening the tech and nanosuit window