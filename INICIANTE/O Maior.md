# #1013 - O Maior

---

## Desafio

Faça um programa que leia três valores e apresente o maior dos três valores lidos seguido da mensagem “eh o maior”. Utilize a fórmula:

$$
MaiorAB = \frac {(a + b + abs (a - b))}{2}
$$

Obs.: a fórmula apenas calcula o maior entre os dois primeiros (a e b). Um segundo passo, portanto é necessário para chegar no resultado esperado.

**Entrada**
O arquivo de entrada contém três valores inteiros.

**Saída**
Imprima o maior dos três valores seguido por um espaço e a mensagem "eh o maior".

---

## Solução

```bash
import java.io.IOException;
import java.util.Scanner;
import java.lang.Math;

public class Main {

    public static void main(String[] args) throws IOException {
        Scanner Scanner = new Scanner(System.in);

        int A = Scanner.nextInt();
        int B = Scanner.nextInt();
        int C = Scanner.nextInt();

        int MaiorAB = (A + B + Math.abs(A - B)) / 2;
        int Maiorv2 = (MaiorAB + C + Math.abs(MaiorAB - C)) / 2;

        System.out.println(Maiorv2 + " eh o maior");

        Scanner.close();
    }
}
```
