# #1019 - Conversão de Tempo

---

## Desafio

Leia um valor inteiro, que é o tempo de duração em segundos de um determinado evento em uma fábrica, e informe-o expresso no formato horas:minutos:segundos.

**Entrada**
O arquivo de entrada contém um valor inteiro N.

**Saída**
Imprima o tempo lido no arquivo de entrada (segundos), convertido para horas:minutos:segundos, conforme exemplo fornecido.

---

## Solução

```java
import java.io.IOException;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) throws IOException {
        Scanner scanner = new Scanner(System.in);

        int tempo = scanner.nextInt();

        int horas = tempo / 3600;
        int resto = tempo % 3600;

        int minutos = resto / 60;
        int segundos = resto % 60;

        System.out.printf("%d:%d:%d\n", horas, minutos, segundos);

        scanner.close();
    }
}
```
