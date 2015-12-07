# m2repository

##Introduction
Mirror Maven repository for Support Libraries and Google Libraries.

### Gradle
Add to your build.gradle:

```gradle
    repositories {
        mavenLocal()
        jcenter()
        mavenCentral()
        maven { url "https://raw.githubusercontent.com/snowdream/mvn-repo/master/releases/" }
        maven { url "https://raw.githubusercontent.com/snowdream/mvn-repo/master/snapshots/" }        
    }
```

###Maven
Add to your pom.xml:
```xml
    <repositories>
        <repository>
            <id>snowdream-nexus-snapshots</id>
            <name>Snowdream Snapshots Repository</name>
            <url>https://raw.githubusercontent.com/snowdream/mvn-repo/master/snapshots/</url>
            <releases>
                <enabled>false</enabled>
            </releases>
            <snapshots>
                <enabled>true</enabled>
            </snapshots>
        </repository>
        <repository>
            <id>snowdream-nexus-releases</id>
            <name>Snowdream Releases Repository</name>
            <url>https://raw.githubusercontent.com/snowdream/mvn-repo/master/releases/</url>
            <releases>
                <enabled>true</enabled>
            </releases>
            <snapshots>
                <enabled>false</enabled>
            </snapshots>
        </repository>        
    </repositories>
```

##License
```
Copyright (C) 2015 Snowdream Mobile <yanghui1986527@gmail.com>

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

        http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
