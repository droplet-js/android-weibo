# android-weibo

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
