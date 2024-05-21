# java.base

[java.base](https://docs.oracle.com/en/java/javase/18/docs/api/java.base/java/io/package-summary.html) 

### 1、BufferedInputStream

提高读取性能，无需重复对底层Input Stream进行操作。还可以对标记当前读取的位置，并在需要时回复到此位置。

```
FileInputStream fileInputStream = new FileInputStream("file.txt");
BufferedInputStream bufferedInputStream = new BufferedInputStream(fileInputStream);
```

