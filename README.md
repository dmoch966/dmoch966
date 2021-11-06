# GoProController Plugin

The GoProController plugin enables remote control of GoPro cameras from DroidScript apps. With this plugin, you can control the camera shutter and change the cameras options.

## Importing and building with Eclipse

Import the project into your Eclipse Workspace:
- File->Import... and select 'Existing Projects into Workspace'
- Browse to your plugin project folder then you should see your plugin project in the 'Projects' list
- Select you plugin project and click Finish

### local.properties

A local.properties file is required in the root of the GoProController folder. This should contain the path to your Android SDK. This can be generated as follows:

`android update project -p [path to GoProController folder]`

Your local.properties file should look something like this:

```
# This file is automatically generated by Android Tools.
# Do not modify this file -- YOUR CHANGES WILL BE ERASED!
#
# This file must *NOT* be checked into Version Control Systems,
# as it contains information specific to your local configuration.

# location of the SDK. This is only used by Ant
# For customization when using a Version Control System, please read the
# header note.
sdk.dir=C:\\Android\\sdk
```

### Building the plugin
- Right-click on pluginBuild.xml and select Run As->Ant Build
- Check the Console for build output

### Installing the plugin
- Make sure your phone is connected via USB and adb is enabled
- Run Install.bat from your plugin project directory
- Launch DroidScript on your phone to complete the install

### Installing the sample App
- Make sure your phone is connected via USB and adb is enabled
- Run the Install.bat file from the GoProController\sample folder
- Restart DroidScript and run the 'GoProController Sample' App
