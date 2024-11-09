# Migrate package name from Java to Kotlin

- Right click java package and choose refactor, rename it to `kotlin`.
- Go to app level `build.gradle.kts` and add the following code block under the `android{}`

```gradle
android {
	android.sourceSets.all {
    	java.srcDir("src/$name/kotlin")
    }
}
```

And then click on Sync Now.
