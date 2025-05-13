# Dialogue-Generator
A dialogue script generator tool in Unity using the LLM Gemini API. In this package includes the tool, example scenes, and free assets from the Unity Asset store. To use this tool, download the .unitypackage file in this repo, and import the package into your Unity project. To open the program interface, click on the "Tools" tab at the top in the toolbar, then "Dialogue Generator.

# Assets
In Assets/Resources/Scenes, Assets/Resources/Characters, and  Assets/Resources/Items are scenes and prefabs for you to test out your dialogue. The assets are imported from the Unity Asset store, and any use of these assets should abide by their respective licenses. After generating a script, place ur characters into the scenes and press play! I have made the main camera to act as the player's POV, so remember to position the camera like a character in the scene as well. 

# API Config
To use the program, you will need an Gemini API key from this website https://ai.google.dev/gemini-api/docs/api-key
Add your key into the JSON file called JSON_KEY_TEMPLATE.json in Assets/Resources/Dialogue, and drag it into the API key field.

The program uses API calls, so if you would like you can replace the model with the http link model of your chocie.

# Context
This section is the initial generation of the script. Drag in NPC and item prefabs to be mentioned in the script. If you want player choices, tick the "player speaking?" box and add a name for the player. Any extra information can be added in the "free prompt" section (e.g. character personality, storyline).
Click generate to generate the script. The compiled file will be in Assets/Resources/Dialoge/TestFile.ink. 

# Add knot
This feature inserts a chapter of story (knot) after the selected knot. Fill in the knot title, and where it will divert to (or leave empty to end the dialogue). Add information about what the knot should talk about in the "Instructions" text field. Click "Add" to add the knot.

# Edit knot
This feature re-generates a selected knot. First select the knot to change.
You can change where the end of the knot diverts to, add a choice, or change a choice's divert (leave any field empty if you don't want any of these aforementioned changes).
Add information about what the knot should talk about in the "Free Prompt" text field. Click "Edit" to edit the knot.

# Delete knot
Select a knot to be deleted. Click "Delete" to delete the selected knot.
