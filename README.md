# Sugar Docker Container

This is a basic docker container to run Sugar.
It should work on GNU/Linux with X11 and pulseaudio.

### Requirements
You just need to have Docker launched

### Usage

#### Launch Sugar (auto detect .activity folders in current directory, persistance is setup via two folders .sugar and .sugar-runner)
```sh
$ sh run.sh
```

![Demo](https://github.com/mikklfr/docker-sugar/raw/master/demo.gif)

#### Launch Sugar and provide folders containing .activity folders
```sh
$ sh run.sh myfolder myfolder2
```

#### Options
- --disable-current-directory # Don't use the current directory to load .activity folders
- --disable-sugar-runner-persistance # Don't map sugar-runner folder
- --disable-sugar-persistance # Don't map sugar folder
- --sugar-persistance folder # Set a folder for .sugar persistance folder
- --sugar-runner-persistance folder # Set a folder for .sugar-runner persistance folder
- --activity folder_containing_activities # Provide folders containing .activity folders
- --resolution 800x600 # setup a custom resolution
