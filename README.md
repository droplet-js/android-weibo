# android-weibo

[![Build Status](https://cloud.drone.io/api/badges/v7lin/android-weibo/status.svg)](https://cloud.drone.io/v7lin/android-weibo)
[ ![Download](https://api.bintray.com/packages/v7lin/maven/weibo-android/images/download.svg) ](https://bintray.com/v7lin/maven/weibo-android/_latestVersion)

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
