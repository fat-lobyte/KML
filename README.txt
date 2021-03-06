KML - Kerbal Markup Lister v0.7.2 - 2017-01-15 (WIP) - A persistence file editor for Kerbal Space Program
KSP Forum: http://forum.kerbalspaceprogram.com/index.php?/topic/133971-win-kml-persistence-file-editor/

Do you face a problem with broken docking ports or need just a little fuel-cheating? Do you got tired of editing save games in a text editor with long loading time and so much scrolling to compare different parts and vessels? So did I and decided to make a more helpful external editor to display the XML-like structure (the "KML" - Kerbal Markup Language) in a tree view and pick out vessels, kerbals and parts to be displayed in more eye-candy way.

The current version is not feature-complete but so far functional and already helps with some problems (or some cheating if you choose to do so).

Any feedback, more testing, bug reports and suggestions are very welcome.

New Features
• new vessel types plane and relay 
• reset docking on one-sided same vessel docking errors - thanks to schneida 
• report only crew assignment problems for kerbals from roster 
• tested with KSP 1.2.2 

Features 
• open SFS and CRAFT files
• save files edited or exactly as loaded
• backup of overwritten files
• display file structure in a "KML" tree
• display all vessels in a sorted and filtered list
• display all kerbals in a sorted and filtered list
• display vessel's part attachment structure
• display warnings about structural problems
• search for nodes, attributes and their content 
• adding, inserting and deleting nodes and attributes
• deletion excludes in current version
  ◦ parts (need to rebuild index numbers and attachments)
• deletion of kerbals and vessels will fix crew assignment 
• support renaming kerbals when assigned 
• send kerbal home to astronaut complex 
• send vessel to low kerbin orbit 
• change vessel flag in all its parts - for Enceos
• refill part resources
• repair broken docking ports and grappling devices
• tested with KSP 1.0, 1.1 and 1.2
  (newest KML version should still work with at least all these KSP versions) 

TODO
• copy nodes and attributes
• identify add-on part connections (KAS)
• change position of nodes and attributes
• more testing (uncommon vessel builds I didn't think of?)
• documentation
• a lot of source code TODOs

Install
• download ZIP file and extract anywhere you want
• run the KML.exe and open your save file
• or choose "open with" on your save file and select KML.exe (command-line arguments supported)

Instructions, Hints, FAQ
• Don't find your vessel in the tree (ordered by in-game creation)? Switch to the "vessels" tab to have a sorted list and the possibility to filter by type (debris, ship, etc.).
• Don't find your kerbal in the tree? There's also a sorted and filtered list in the "kerbals" tab.
• Want to see how the parts of your vessel are connected? Have a look on the graph displayed in the "vessels" tab.
• What do the colored lines in that part graph mean?
  ◦ Dark green line is a node attachment in top/down direction
  ◦ Light green is a node attachment in front/back or left/right direction
  ◦ Yellow line is a surface attachment
• If parts are arranged in a way you can't see where the connections go, mouse over the part and they are drawn thicker.
• After you found your vessel, kerbal or part in the list you want to see it in the tree? Just make a double click.
• Sometimes there appears a warnings tab, what do these warnings mean? Some KML elements are more heavily inspected than others, like vessel parts and especially docking or grappling devices. If something is not as expected there is a warning generated.
• There is a warning but my save game works fine! If the problem is related to stock parts please send me feedback about this problem. If KML has warnings about add-on parts not connected (e.g. KAS): That's ok for now, KML does not support that add-on and can't understand what it has written to the save file. KML just expects all parts to be somehow connected and gives a warning otherwise.
• Don't fear about saving a file with warnings, unknown add-ons, missing part-connections, etc. KML will save the file as it was read and only apply the changes you made. All unknown data will be kept as it was.
