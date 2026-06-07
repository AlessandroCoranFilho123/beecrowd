# #1010 - Cálculo Simples

---

## Desafio

Neste problema, deve-se ler o código de uma peça 1, o número de peças 1, o valor unitário de cada peça 1, o código de uma peça 2, o número de peças 2 e o valor unitário de cada peça 2. Após, calcule e mostre o valor a ser pago.

**Entrada**
O arquivo de entrada contém duas linhas de dados. Em cada linha haverá 3 valores, respectivamente dois inteiros e um valor com 2 casas decimais.

**Saída**
A saída deverá ser uma mensagem conforme o exemplo fornecido abaixo, lembrando de deixar um espaço após os dois pontos e um espaço após o "R$". O valor deverá ser apresentado com 2 casas após o ponto.

---

## Solução

```bash
import java.io.IOException;
import java.util.Scanner;
import java.lang.Math;

public class Main {

    public static void main(String[] args) throws IOException {
        Scanner Scanner = new Scanner(System.in);

        int code1 = Scanner.nextInt();
        int number1 = Scanner.nextInt();
        double value1 = Scanner.nextDouble();

        int code2 = Scanner.nextInt();
        int number2 = Scanner.nextInt();
        double value2 = Scanner.nextDouble();

        double total = (number1 * value1) + (number2 * value2);

            System.out.printf("VALOR A PAGAR: R$ %.2f%n", total);

        Scanner.close();
    }
}
```
