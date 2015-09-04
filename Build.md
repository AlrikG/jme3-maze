## JMonkeyEngine (JME3) Software Development Kit (SDK) ##

  * Download the jMonkeyEngine SDK from http://hub.jmonkeyengine.org/downloads
  * Install the SDK, which includes:
    * the engine itself,
    * an integrated development environment (IDE) based on NetBeans, and
    * the Blender 3D application.

The hardware and software requirements of the SDK are documented at http://hub.jmonkeyengine.org/wiki/doku.php/jme3:requirements

## Plugins ##

You will need the following plugins:  [tonegodGUI](http://hub.jmonkeyengine.org/wiki/doku.php/jme3:contributions:tonegodgui) and [SkyControl](https://code.google.com/p/jme3-utilities/wiki/SkyControl).  These can be downloaded from the "jMonkeyPlatform User Contributions" update center.

To install plugins:
  * Open the Plugins dialog in the IDE:
    * Menu bar -> "Tools" -> "Plugins"
  * Click on the "Settings" tab.
  * Make sure the box next to "JMonkeyEngine SDK User Contributions" is checked.
    * If it isn't, check the box.
  * Click on the "Available Plugins" tab.
  * Click on the "Name" button in the header to sort by name.
  * Check the "Install" box next to each plugin you wish to install.
  * Click on the "Install" button.
  * Follow the instructions of the Plugin Installer wizard, (reading and) accepting all license agreements.

It's normal to get a validation warning telling you that the plugins are unsigned.  It's normal to restart the IDE after installing plugins.

## Source files ##

Check out the Maze Game source files using Subversion:
  * Open the Checkout wizard in the IDE:
    * Menu bar -> "Team" -> "Subversion" -> "Checkout..."
  * For "Repository URL:" specify "http://jme3-maze.googlecode.com/svn" (without the quotes).
  * Clear the "User:" and "Password:" text boxes.
  * Click on the "Next >" button.
  * For "Repository Folder(s):" specify "trunk" (without the quotes).
  * For "Local Folder:" specify a writable folder on a local filesystem or a non-existent subfolder of such a folder.
  * Make sure the "Skip ... and checkout only its content" box is checked.
  * Make sure the "Scan for NetBeans Projects after Checkout" box is checked.
  * Click on the "Finish" button.
  * When asked whether to open the project, click the "Open Project" button.

## Project configuration ##

  * (optional) Rename the project:
    * Right-click on the "maze" project in the "Projects" window.
    * Select "Rename...".
    * Type a new name in the text box.
    * Click on the "Rename" button.
  * Build the project's JARs:
    * Right-click on the new project in the "Projects" window.
    * Select "Clean and Build".
  * (optional) Generate the project's javadoc:
    * Right-click on the new project in the "Projects" window.
    * Select "Generate Javadoc".

## Asset conversion ##

Before you run the game itself, you'll need to convert the Blender assets to native format.  To do this, run the AssetProcessor.java file in the jme3maze package.

Note:  The source files are in JDK 7 format, but the IDE creates new JME3 projects in JDK 5 format.