# Android library Publishing
Publishing your own android library to local maven repository.

## Create a android project

Add a new module for your created project. Name the module as you wish and that will be your library project for the created android project.

## Adding maven plugin

In your project level build.gradle add  
``` classpath 'com.github.dcendents:android-maven-gradle-plugin:1.3'```

In your library project or module's build.gradle add  
``` apply plugin: 'com.github.dcendents.android-maven'```

You can also add 

``` group = 'com.develops' ```
``` version = '1.0' ```

## Pushing to local maven

Once all done run this command in terminal

``` gradlew install ```

Now you can use your library as gradle dependency in any of your android project

``` compile ('com.develops:yourlibraryname:1.0')```

For more info look at this

[https://github.com/dcendents/android-maven-gradle-plugin]
