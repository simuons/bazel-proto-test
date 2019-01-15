`bazel build :b_java_proto` gives

```
* bazel-bin/liba-speed.jar
         0 Fri Jan 01 00:00:00 EET 2010 META-INF/
       105 Fri Jan 01 00:00:00 EET 2010 META-INF/MANIFEST.MF
       971 Fri Jan 01 00:00:02 EET 2010 AOuterClass$1.class
      1243 Fri Jan 01 00:00:02 EET 2010 AOuterClass$A$1.class
     11825 Fri Jan 01 00:00:02 EET 2010 AOuterClass$A$Builder.class
     10830 Fri Jan 01 00:00:02 EET 2010 AOuterClass$A.class
       219 Fri Jan 01 00:00:02 EET 2010 AOuterClass$AOrBuilder.class
      2762 Fri Jan 01 00:00:02 EET 2010 AOuterClass.class
* bazel-bin/libb-speed.jar
         0 Fri Jan 01 00:00:00 EET 2010 META-INF/
       105 Fri Jan 01 00:00:00 EET 2010 META-INF/MANIFEST.MF
       971 Fri Jan 01 00:00:02 EET 2010 BOuterClass$1.class
      1243 Fri Jan 01 00:00:02 EET 2010 BOuterClass$B$1.class
     11825 Fri Jan 01 00:00:02 EET 2010 BOuterClass$B$Builder.class
     10826 Fri Jan 01 00:00:02 EET 2010 BOuterClass$B.class
       219 Fri Jan 01 00:00:02 EET 2010 BOuterClass$BOrBuilder.class
      2762 Fri Jan 01 00:00:02 EET 2010 BOuterClass.class
* bazel-genfiles/b-speed-src.jar
     15565 Tue Jan 01 00:00:00 EET 1980 BOuterClass.java
        50 Tue Jan 01 00:00:00 EET 1980 META-INF/MANIFEST.MF
```
