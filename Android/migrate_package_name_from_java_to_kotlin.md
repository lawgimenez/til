# Migrate package name from Java to Kotlin

- Right click Java package and choose refactor, rename it to `Kotlin`.
- Go to app level `build.gradle.kts` and add the following code block under the `android{}`

```
android {
	android.sourceSets.all {
    	java.srcDir("src/$name/kotlin")
    }
}
```

And then click on Sync Now.
