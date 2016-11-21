# export-import-external-jar-in-eclipse
creating external libraries related to game engine as a sample game enigne

Aim:
I wanna add rgsconfig as an external library to a sample game engine.

Steps:
1. right click rgsconfig project -> export -> Jar file -> next 
    -> select files I wanna include in the jar -> destination -> finish
2. alternative to step2, put the .jar in libs, if there is no such libs folder, create one. 
    (It's becoz build.gradle has set to read all .jars in libs with the line below:
        compileOnly fileTree(dir: 'libs', include: '*.jar')
3. refresh gradle dependencies / refresh all
4. external jar should exist in Gradle Dependencies folder
