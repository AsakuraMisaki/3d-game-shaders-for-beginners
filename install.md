# Building With Windows VS studio
[thanks:https://www.bilibili.com/read/cv11695886]
- require:
    - vs studio 2017+
    - panda3d sdk (c++)
    - source code
- steps:
    - git or download the source code
    - get panda3d sdk
    - vs studio: create project with the existed source code 
    - project properties: 
        - add includes path
            - if errors with xxx.h and the h is in the sub folder of the include folder, just parse it into the root include folder.
            ![](/docs/steps/include.webp)
        - add libs path
            ![](/docs/steps/lib.webp)
        - add lib refers name: complete here
            - libp3framework.lib  
            libpanda.lib   
            libpandafx.lib  
            libpandaexpress.lib  
            libpandaphysics.lib  
            libp3dtool.lib  
            libp3dtoolconfig.lib  
            libp3pystub.lib  
            libp3direct.lib
            ![](/docs/steps/lib_names.webp)  
        - release, not debug (panda has no debug support)
            ![](/docs/steps/release.webp)
        - use the unix path syntax to load shaders
            ![](/docs/steps/unix.webp)
    - release and enjoy
