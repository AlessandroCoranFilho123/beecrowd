# #1015 - Distância Entre Dois Pontos

---

## Desafio

Leia os quatro valores correspondentes aos eixos x e y de dois pontos quaisquer no plano, p1(x1,y1) e p2(x2,y2) e calcule a distância entre eles, mostrando 4 casas decimais, segundo a fórmula:

Distancia = $\sqrt{(x_2 - x_1)^2 + (y_2 - y_1)^2}$

**Entrada**
O arquivo de entrada contém duas linhas de dados. A primeira linha contém dois valores de ponto flutuante: x1 y1 e a segunda linha contém dois valores de ponto flutuante x2 y2.

**Saída**
Calcule e imprima o valor da distância segundo a fórmula fornecida, considerando 4 casas decimais.

---

## Solução

```bash
import java.io.IOException;
import java.util.Scanner;
import java.lang.Math;

public class Main {

    public static void main(String[] args) throws IOException {
        Scanner Scanner = new Scanner(System.in);

        double x1 = Scanner.nextDouble();
        double y1 = Scanner.nextDouble();
        double x2 = Scanner.nextDouble();
        double y2 = Scanner.nextDouble();

        double x = (x2 - x1) * (x2 - x1);
        double y = (y2 - y1) * (y2 - y1);
        double Distancia = Math.sqrt(x + y);

        System.out.printf("%.4f%n", Distancia);

        Scanner.close();
    }
}
```
