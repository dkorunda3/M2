## Information of `build.gradle`

```
dependencies {
    compile files('lib/resources.jar')
}
```
This is for compiling.

```
jar {
    manifest {
        attributes 'Main-Class': 'edu.gatech.oad.antlab.pkg1.AntLabMain',
                   'Class-Path': 'lib/resources.jar'
    }
    destinationDir = file('.')
}
```
This is for compiled jar file.

In this configuration, jar file will be generated at the top directory, and can be directly run by `java -jar`.
