# How to get
add jitpack repo:
```
repositories {
    maven { url "https://jitpack.io" }
}

*.kts
repositories {
    maven { setUrl("https://jitpack.io") }
}
```
add dependency:
```
implementation 'com.github.luca992:coil-composable:{version}'

*.kts:
implementation("com.github.luca992:coil-composable:{version}")
```
[![](https://jitpack.io/v/luca992/coil-composable.svg)](https://jitpack.io/#luca992/coil-composable)

# How to use
```
CoilImage("url")
```

or if you want more control
```
CoilImage("url") {
    // this LoadRequestBuilder
    placeholder(
        ResourcesCompat.getDrawable(
            context.resources,
            R.drawable.loading_indicator,
            null
        )
    )
}
```
