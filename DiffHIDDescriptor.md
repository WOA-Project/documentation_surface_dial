# Diff between Default and Overwritten

```
38c38,39
< 0x25, 0x00,        //       Logical Maximum (0)
---
> 0x26, 0x80, 0x25,  //       Logical Maximum (9600)
> 0x46, 0x63, 0x0C,  //       Physical Maximum (3171)
42a44,45
> 0x26, 0x20, 0x1C,  //       Logical Maximum (7200)
> 0x46, 0x42, 0x08,  //       Physical Maximum (2114)
154c157
< // 319 bytes
\ No newline at end of file
---
> // 329 bytes
\ No newline at end of file
```