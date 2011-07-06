murmurhash-java
=================

this is an implementation by Viliam Holub of the fast non-cryptographic **murmur hash** algorithm. it is written in java and is implemented in both 32 and 
**64-bit** versions. 

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
