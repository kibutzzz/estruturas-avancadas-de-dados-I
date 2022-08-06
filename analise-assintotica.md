# Analise assintotica - Exercicios: Qual a ordem?
1.1
| ----------------------------- | Melhor = Pior =  Medio |
| ----------------------------- | ---------------------- |
| int conta = 0                 |           1            |
| for(int i = 0; i < n; i++)    |          n+1           |
|   for(int j = 0; j < n; j ++) |         n^2+n          |
|     conta++;                  |          n^2           |
| t(n)                          |      2n^2 + 2n + 2     |
| O(n)                          |           n^2          |

1.2

|---                          | Melhor=Pior=Medio |
|---                          |   ---             |
|int conta = 0;               |        1          |
|int i = 1;                   |        1          |
|while(i < n) {               |        n          |
| for(int j = 0; j < n; j++)  |      n^2 - 1      |
|   conta++;                  |      n^2 -n       |
| i++;                        |       n-1         |
|       t(n)                  |       2n^2        |
|       O(n)                  |        n^2        |