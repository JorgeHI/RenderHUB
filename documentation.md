# Render HUB Documentation

## Management

<img src="https://github.com/user-attachments/assets/c831488e-8abe-4606-a1e7-d28ae923dfb5" width="60%" align="right">

Mode: You can select the current mode of the HUB. The node have 3 posible values:

- Work: The High cost nodes will be disable and the working profile will be used for the knob values.
- Render: All the nodes will be active and the Render profile will be used for the knob values.
- Auto-$gui: This mode select automatically the work mode when Nuke is in interface mode and Render mode when it’s in batch mode, like the $gui expression. It’s usefull for pipeline environment with a render farm system.

Select Actions: This option are usefull to select all the High cost nodes of a specific type in your script or all the nodes parent to the HUB or a specific node type parent to the HUB. With this option you can keep the track of what you have parent to the node, even if you have the Hide link option active.

Parent Actions: The best part, parent you nodes to the HUB!
- Hide links: If you active this checkbox, the links will be hidden to keep you script clean (The Hide link option onle works with the Disable knobs and the Switch nodes at the moment). This option will make a 2 point parent between the Node, the Root (Project settings) and the HUB.
- Parent & Unparent: Option to parent a Node or a knob of a Node.
  - If you set Auto mode, the action will parent the nodes depending of their type (Switch, Transform or the Disable knob for other node type)
  - You can choose between the Parent or the Unparent option to parent a new Node or unparent a Node.
  - You can select an specific user profile to parent the nodes, if you don't have User profiles created check the Profiles tab to configure them.
  - When you pressed the button, the selected nodes will be parent or unparent to/from the HUB.
  
Script cleaning: This Node can generate a lot of expressions and a custom knobs in the Root of your script, if you want to clean your script of any conexion or modification that this Node could be cause to your Nuke script, you only need to press this button. When you press it, it will ask you if you are sure to remove all the links and set the values of the current mode.
- If you are in Work mode, when you execute the cleaning, the Work values will be set in all the parent nodes. In the other hand, if you execute the cleaning in the Render mode, the Render values will be set in the nodes.

## General

<img src="https://github.com/user-attachments/assets/f759735f-b786-451f-9d82-e9ce740ab205" width="70%" align="left">

This properties tab containg all the knobs used in the basic profile. This profile is used for the parent of filter and motion blur knobs. 
Like you would have in a custom user profile, you have the work config sectio nand the render config section. You can define your work and render mode values for each knob here.
<br><br><br><br><br><br><br><br><br><br>

## Profiles

<img src="https://github.com/user-attachments/assets/f28ea812-aa5b-4ba1-9109-d47ed5626627" width="50%" align="right">

In this properties tab you will find the utilities to create you own node profiles.
You can create as many node profiles as you want. To create a Node profile the only requirements are a profile name, must be unique in the Render HUB node, and a node type for the profile. You have a editable combobox to select the node type for the profile. If you don't find the node type that you want to create in the list, you can write the type manually, or select a node of that type and use the button "Add selected node type" to append the node type of your selected node to the list of types to create profiles.

When the profile is create the will find a new tab in the node with the profile name, you can configure the profile on it.

Like you will be able to have several profiles, this tab also have some utilities to manage them. Under the profile creation section you have a combobox with the list of profiles currently created in the Node. You can select one of the profiles to check the node type of the profile and which nodes from you Nuke script are parent to this specific profile. This will help you to understand the current use of each profile. In this section you have the button to remove a profile too. If you want to remove a profile, make sure that the profile is not being used before remove it, otherwise you can end having expressions in the nodes that does not work anymore.



## User Profile (ScanlineRender example)

<img src="https://github.com/user-attachments/assets/35d38001-c9f3-4c58-bb4a-b960d460a4cc" width="70%" align="left">

For each profile that you create you will have a tab. Each tab will be different, because the profiles tabs are cre4ated dynamicaly from the node type selected to have the knobs from that node type. However, you will have always a work and a render config sections. You can configure a value for each knob in both modes. A part from that, you have a button to restor the knob values from a mode section to default.
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>

## Help

![image](https://github.com/user-attachments/assets/d13d4515-1514-4db9-96bd-9effeac93683)

In the help tab you will find some information about the Node. Like the version of the node and a email for support.
Also, you will find some buttons:
- Documentation: It links to the documentation of the node.
- Nukepedia: It links to the Nukepedia page of Render HUB
- Report Problem: It open the report Issue page of github in the Render HUB project, ready to create a new Issue.

