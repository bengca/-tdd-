![Image text](https://github.com/bengca/-tdd-/blob/main/img/20210219.png1)

# 一. **数据类型**

| 类型    | 二进制位数 | 最大存储数据量 | 数据范围                        | 包装类  |
| ------- | ---------- | -------------- | ------------------------------- | ------- |
| byte    | 8          | 255            | -128~127之间                    | Byte    |
| short   | 16         | 65536          | -32768~32767之间                | Short   |
| int     | 32         | 2的32次方减1   | 负的2的31次方到正的2的31次方减1 | Integer |
| lang    | 64         | 2的64次方减1   | 负的2的63次方到正的2的63次方减1 | Long    |
| float   | 32         |                | 3.4e-45~1.4e38                  | Float   |
| double  | 64         |                | 4.9e-324~1.8e308                |         |
| boolean | 1          | true/false     |                                 |         |

1. 字符串类型，String，不是基础类型。其实是由一个字符数组来构成。

2. 基础类型的特点:全部小写，是Java内置的关键字(不同颜色显示)，同时是CPU可以直接处理的类型。

3. 基础类型的取值范围:

  a)1字节(byte)=8位(bit)二进制位，100Mbps = 100M bit per second = 12.5MByte.b)1字节的范围=.0000 0000~11111111 =0~255共256个，2^8。
  b)1字节的范围 = 0000 0000~1111 1111 = 0 ~ 255 共256个，2^8。

  c)byte型是属于有符号类型，会将第一位用于表示正负号，0表示正数，1表示负数。

  d)O0000 000~O1111 111 =>0~127 -127~-0, +0~+127 => -128 => -128~0~127 = 256个。

  e) short类型:16位，2^16=65536个。

  f)int类型:32位，2432=4294967296个。

  g)long长整型:64，2^64个。
  h)在Java 中，只有 char类型是无符号类型，2字节65536个，0~65535。
  i)char用于表示一个字符，这个字符可以是中文或ASCIl码，char 与int可以完全对等转换。

4. 数据类型的强制转换：

  - 小范围的类型转换为大范围的类型，不需要强制转换。
  - 大范围类型转换为小范围类型，默认是不允许的，但是可以进行强制转换（但是可能导致取值异常）。
  - 在JS或Python中，X=1000000000；JS，默认都是处理为64位。对内存赤裸裸的浪费。

5. 引用类型:变量定义在堆内存中，通过栈内存的指针进行引用进而操作该变量的方式。
  比如一个数组 int[]，一个字符串 String，或者是自定义的类:FirstDemo。

