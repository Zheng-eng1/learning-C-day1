# learning-C-day1
day-1
#include<studio.h>
int main <void>
{
int i = 9;
printf("%d",i * i);\\修改前printf("i * i\n" , i );\\需要有占位符%d 
return 0 ;
}

# 运算符
#include <stdio.h>
int main()
{
    int a = 17, b = 5, count = 0;

    printf("a + b = %d\n", a + b);          // 加法: 22
    printf("a - b = %d\n", a - b);          // 减法: 12
    printf("a * b = %d\n", a * b);          // 乘法: 85
    printf("a / b = %d\n", a / b);          // 整数除法(商): 3
    printf("a %% b = %d\n", a % b);         // 取模(余数): 2
    printf("a / b = %.2f\n", (float)a / b); // 浮点除法: 3.40
    printf("(double)a / b = %.3f\n", (double)a / b); // 浮点除法: 3.400

    printf("a > b = %d\n", a > b);          // 关系运算: 1(真)
    printf("a == b = %d\n", a == b);        // 相等判断: 0(假)
    printf("condition range: %d\n", a >= 0 && a <= 100); // 范围判断: 1

    count = 0;
    printf("0 && count = %d\n", 0 && count);            // 左假短路，右边不执行，结果0
    printf("count after left short-circuit = %d\n", count); // count仍为0

    printf("1 || count = %d\n", 1 || count);            // 左真短路，右边不执行，结果1
    printf("count after right short-circuit = %d\n", count); // count仍为0

    printf("bitwise AND: %d\n", 7 & 8);     // 按位与: 0111 & 1000 = 0
    printf("bitwise OR:  %d\n", 7 | 8);     // 按位或: 0111 | 1000 = 15
    printf("bitwise XOR: %d\n", 7 ^ 8);     // 按位异或: 0111 ^ 1000 = 15
    printf("left shift:  %d\n", 1 << 3);    // 左移3位: 1→8

    return 0;
}
