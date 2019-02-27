# android-weibo

[![Build Status](https://cloud.drone.io/api/badges/v7lin/android-weibo/status.svg)](https://cloud.drone.io/v7lin/android-weibo)
[![GitHub tag](https://img.shields.io/github/tag/v7lin/android-weibo.svg)](https://github.com/v7lin/android-weibo/releases)
[![API](https://img.shields.io/badge/API-14%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=14)

### snapshot

````
ext {
    latestVersion = '1.0.0-SNAPSHOT'
}

allprojects {
    repositories {
        ...
        // weibo
        maven {
            url "https://dl.bintray.com/thelasterstar/maven/"
        }
        
        maven {
            url 'https://oss.jfrog.org/artifactory/oss-snapshot-local'
        }
        ...
    }
}
````

### release

````
ext {
    latestVersion = '1.0.0'
}

allprojects {
    repositories {
        ...
        jcenter()
        
        // weibo
        maven {
            url "https://dl.bintray.com/thelasterstar/maven/"
        }
        ...
    }
}
````

### usage

android
````
...
dependencies {
    ...
    implementation "io.github.v7lin:weibo-android:${latestVersion}"
    ...
}
...
````
