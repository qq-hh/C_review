### #pragma预处理分析

![image-20231028192310013](文档中本地图片/image-20231028192310013.png)

内存对齐

![image-20231030195619968](文档中本地图片/image-20231030195619968.png)

![image-20231030195838866](文档中本地图片/image-20231030195838866.png)

![image-20231105194244029](文档中本地图片/image-20231105194244029.png)

```
#include <stdio.h>
 
#pragma pack(8)
 
struct S1
{
    short a;
    long b;
};
 
struct S2
{
    char c;
    struct S1 d;
    double e;
};
 
#pragma pack()
 
int main()
{
    struct S2 s2;
     
    printf("%d\n", sizeof(struct S1));
    printf("%d\n", sizeof(struct S2));
    printf("%d\n", (int)&(s2.d) - (int)&(s2.c));
 
    return 0;
}
```

