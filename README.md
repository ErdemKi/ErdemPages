# ErdemPages
ErdemPages is a Maven repository hosted using GitHub Pages for my Minecraft mods.
## Available Mods & Versions
For available mods and versions, please see the [com/erdem](com/erdem) directory.
## Usage
### `build.gradle`
First, add the repository link to the `repositories` block:
````groovy
repositories {
    maven {
        name = "ErdemPages"
        url = uri("https://erdemki.github.io/ErdemPages")
    }
}
````
`name` is the name inside the Gradle and can be changed. URL must remain unchanged.

Then add the mod you want to use to the `dependencies` block:
````groovy
dependencies {
    //other dependencies
    modImplementation "com.erdem:<artifact_id>:<mod_version>"
}
````

`artifact_id` is the ID of artifact.

`mod_version` is the version of the mod.

For artifact ID and available versions, please see [Available Mods & Versions](#available-mods--versions).
### `build.gradle.kts`
First, add the repository link to the `repositories` block:
````kotlin
repositories {
    maven {
        name = "ErdemPages"
        url = uri("https://erdemki.github.io/ErdemPages")
    }
}
````
`name` is the name inside the Gradle and can be changed. URL must remain unchanged.

Then add the mod you want to use to the `dependencies` block:
````kotlin
dependencies {
    //other dependencies
    modImplementation("com.erdem:<artifact_id>:<mod_version>")
}
````

`artifact_id` is the ID of artifact.

`mod_version` is the version of the mod.

For artifact ID and available versions, please see [Available Mods & Versions](#available-mods--versions).