# javabuild

This is a simple [shellfire] application to ease the command line building of Java code organised in IntelliJ modules. It is not designed as a full build system, with dependencies, etc. It was born out of a need to compile JDK-replacement classes and produce simple, non-JAR output.

Since development is undertaken by this author using IntelliJ, many of the features of a Java compiler are of no interest (eg warnings, treating errors as warnings (particulary as `javac` has often been incorrect with these), etc).

## Notes

* The order of entries in a module (`.iml` file) is ignored. Instead, libraries are placed before module dependencies.
* We ignore `exported=""` and assume all modules are exported. This is more liberal.
