# 编译原理 第14次作业

**151220129 计科 吴政亿 wuzy.nju@gmail.com**

## 第一题 9.2.1

1. |       | gen   | kill    |
   | ----- | ----- | ------- |
   | $B_1$ | 1,2   | 8,10,11 |
   | $B_2$ | 3,4   | 5,6     |
   | $B_3$ | 5     | 4,6     |
   | $B_4$ | 6,7   | 4,5,9   |
   | $B_5$ | 8,9   | 2,7,11  |
   | $B_6$ | 10,11 | 1,2,8   |

2. |       | In              | Out           |
   | ----- | --------------- | ------------- |
   | $B_1$ | $\emptyset$     | 1,2           |
   | $B_2$ | 1,2,3,5,8,9     | 1,2,3,4,8,9   |
   | $B_3$ | 1,2,3,4,6,7,8,9 | 1,2,3,5,7,8,9 |
   | $B_4$ | 1,2,3,5,7,8,9   | 1,2,3,6,7,8   |
   | $B_5$ | 1,2,3,5,7,8,9   | 1,3,5,8,9     |
   | $B_6$ | 1,3,5,8,9       | 3,5,9,10,11   |

   

## 第二题 9.2.3

1. |       | def   | use    |
   | ----- | ----- | ------- |
   | $B_1$ | a,b | $\O$ |
   | $B_2$ | c,d | a,b   |
   | $B_3$ | $\O$ | b,d   |
   | $B_4$ | d   | a,b,e |
   | $B_5$ | e   | a,b,c |
   | $B_6$ | a | b,d |

2. |       | In        | Out       |
   | ----- | --------- | --------- |
   | $B_1$ | e         | a,b,e     |
   | $B_2$ | a,b,e     | a,b,c,d,e |
   | $B_3$ | a,b,c,d,e | a,b,c,d,e |
   | $B_4$ | a,b,c,e   | a,b,c,d,e |
   | $B_5$ | a,b,c,d   | a,b,d     |
   | $B_6$ | b,d       | $\O$      |