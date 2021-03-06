# Guild

Simple java tuples.

Guild offers you tuple classes from two to four elements.

* [Pair](https://github.com/operando/Guild/blob/master/guild/src/main/java/com/os/operando/guild/Pair.java)
 * A tuple of two elements.
* [Triplet](https://github.com/operando/Guild/blob/master/guild/src/main/java/com/os/operando/guild/Triplet.java)
 * A tuple of three elements.
* [Quartet](https://github.com/operando/Guild/blob/master/guild/src/main/java/com/os/operando/guild/Quartet.java)
 * A tuple of four elements.

## Download

[![Download](https://api.bintray.com/packages/operandoos/maven/guild/images/download.svg?version=1.0.0) ](https://bintray.com/operandoos/maven/guild/1.0.0/link) or grab via Gradle:

```gradle
compile 'com.os.operando.guild:guild:1.0.0'
```

or Maven:

```
<dependency>
  <groupId>com.os.operando.guild</groupId>
  <artifactId>guild</artifactId>
  <version>1.0.0</version>
</dependency>
```

## How to use

### Pair

```java
Pair<String, Integer> pair = Pair.create("pair", 0);
System.out.println(pair.getFirst());
System.out.println(pair.getSecond());
```

### Triplet

```java
Triplet<String, Integer, Boolean> triplet = Triplet.create("triplet", 0, false);
System.out.println(triplet.getFirst());
System.out.println(triplet.getSecond());
System.out.println(triplet.getThird());
```

### Quartet

```java
Quartet<String, Integer, Boolean, LocalDate> quartet = Quartet.create("triplet", 0, false, LocalDate.now());
System.out.println(quartet.getFirst());
System.out.println(quartet.getSecond());
System.out.println(quartet.getThird());
System.out.println(quartet.getFourth());
```

## Future

Guild supports up to nine elements in the future.

The class name is expected to be the same as the [javatuples](http://www.javatuples.org/).

### License

```
Apache Version 2.0

Copyright (C) 2016 Shinobu Okano

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