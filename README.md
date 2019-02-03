# GameLauncher
Game launching tool for Java-based games

# How it works:

The engine interacts with resource repositories over HTTP, as you can customize the endpoints and the log entries.   
The tool automatically creates the required directories and reads the pre-defined text files, that you must create at your repository destination. These should contain single text lines with all the resources that you use in your game classes. You will find an example inside the project repo.   

 

# Initial structure:

The tool consists of two classes:   

**Launcher.java**, responsible for the online streaming and loading of the downloaded resources   
**UpdateLog.java**, responsible for the generation and beautifying of the created log file, containing all streamed resources and their modifications   

The default resource files and folders are:   

**images/images.txt** - contains the description of the images, that are used   
**sounds/sounds.txt** - contains the description of the sounds, that are used   
**version.txt** - contains the version of the compiled game; if the local version matches the version in the remote repository, then "up-to-date" is written inside the local version.txt   

NB.: Of course, you could extend this structure further, so that it fits to your project.
