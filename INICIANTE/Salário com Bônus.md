# #1009 - Salário com Bônus

---

## Desafio

Faça um programa que leia o nome de um vendedor, o seu salário fixo e o total de vendas efetuadas por ele no mês (em dinheiro). Sabendo que este vendedor ganha 15% de comissão sobre suas vendas efetuadas, informar o total a receber no final do mês, com duas casas decimais.

**Entrada**
O arquivo de entrada contém um texto (primeiro nome do vendedor) e 2 valores de dupla precisão (double) com duas casas decimais, representando o salário fixo do vendedor e montante total das vendas efetuadas por este vendedor, respectivamente.

**Saída**
Imprima o total que o funcionário deverá receber, conforme exemplo fornecido.

---

## Solução

```bash
import java.io.IOException;
import java.util.Scanner;
import java.lang.Math;

public class Main {

    public static void main(String[] args) throws IOException {
        Scanner Scanner = new Scanner(System.in);

        String nome = Scanner.nextLine();
        double B = Scanner.nextDouble();
        double C = Scanner.nextDouble();

        double total = B + (C * 0.15);

            System.out.printf("TOTAL = R$ %.2f%n", total);

        Scanner.close();
    }
}
```
