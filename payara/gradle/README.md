# Payara
This scripts downloads, extracts and configures the latest version of the JavaEE compatible application server [Payara](https://payara.fish)
# Usage
Execute the whole chain of commands with the following commands on Windows ...
```
.\gradlew.bat dDD
```
... or Linux.
```
chmod u+x ./gradlew
./gradlew dDD
```
After completion Payara resides in "build\unpacked\payara".
# Hints
dDD is an abbreviation for "deleteDefaultDomains". Gradle can handle such abbreviations and it makes calling commands shorter and easier. The dependency chain calls all required tasks back to clean because they are defined in the Script with the directive "dependsOn" in each task.