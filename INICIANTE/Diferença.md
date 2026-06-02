# #1007 - Diferença

---

## Desafio

Leia quatro valores inteiros A, B, C e D. A seguir, calcule e mostre a diferença do produto de A e B pelo produto de C e D segundo a fórmula: DIFERENCA = (A _ B - C _ D).

**Entrada**
O arquivo de entrada contém 4 valores inteiros.

**Saída**
Imprima a mensagem DIFERENCA com todas as letras maiúsculas, conforme exemplo abaixo, com um espaço em branco antes e depois da igualdade.

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
        int D = Scanner.nextInt();

        int diferenca = (A * B) - (C * D);

        System.out.println("DIFERENCA = " + diferenca);

        Scanner.close();
    }
}
```
