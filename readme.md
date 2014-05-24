murmurhash-java
=================

This is an implementation by Viliam Holub of the fast non-cryptographic **murmurhash2** algorithm. 

It is written in Java and is implemented in both 32 and **64-bit** versions. 

If you want the latest in the world of murmur, check out Guava's [Hashing](http://docs.guava-libraries.googlecode.com/git-history/master/javadoc/com/google/common/hash/Hashing.html) class, 
which has 32 and 128 bit implementations of **murmur3**.

building
----------

Build a package with `maven`:

```
mvn package
```

Run the tests:

```
mvn test
```

public api
--------------

```java

public final class MurmurHash {
    public static int  hash32(final byte[] data, int length);
    public static long hash64(final byte[] data, int length);
    public static int  hash32(final byte[] data, int length, int seed);
    public static long hash64(final byte[] data, int length, int seed);
    public static int  hash32(final String text);
    public static long hash64(final String text);
    public static int  hash32(final String text, int from, int length);
    public static long hash64(final String text, int from, int length);
}

```

author
---------

This code was released by Viliam into the public domain. [More information is here](http://d3s.mff.cuni.cz/~holub/sw/javamurmurhash/).
