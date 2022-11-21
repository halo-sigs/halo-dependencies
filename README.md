## halo-dependencies

Halo dependencies is a library that provides a simple way to manage dependencies in your project.

### How to publish
```shell
export OSSR_USERNAME=your-maven-repo-username
export OSSR_PASSWORD=your-maven-repo-password
./gradlew publish
```

### How to use it
Add the following lines to your `build.gradle` file:

```groovy
repositories {
    mavenCentral()
    maven { url 'https://s01.oss.sonatype.org/content/repositories/snapshots/' }
}

dependencies {
    implementation platform('run.halo.dependencies:halo-dependencies:1.0.0-SNAPSHOT')
    // ...
}
```
