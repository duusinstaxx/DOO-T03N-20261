# Paradigmas de Programação: Imperativo vs Declarativo

Os paradigmas de programação definem a forma como um programa é estruturado e executado. Entre os principais paradigmas estão o imperativo e o declarativo, que diferem na maneira como as instruções são fornecidas ao computador.

## Paradigma Imperativo

No paradigma imperativo, o programador descreve passo a passo como o problema deve ser resolvido, especificando claramente o fluxo de execução.

## Paradigma Declarativo

No paradigma declarativo, o foco está em o que deve ser feito, sem detalhar o processo de execução. O sistema se encarrega de encontrar a solução.

## Comparação: Java (Imperativo) vs Prolog (Declarativo)

### Cálculo de Fatorial

**Imperativo (Java)**

```java
public class Fatorial {
    public static int fatorial(int n) {
        int resultado = 1;
        for (int i = 1; i <= n; i++) {
            resultado *= i;
        }
        return resultado;
    }
    public static void main(String[] args) {
        System.out.println(fatorial(5));
    }
}
```

**Declarativo (Prolog)**

```prolog
fatorial(0, 1).
fatorial(N, F) :-
    N > 0,
    N1 is N - 1,
    fatorial(N1, F1),
    F is N * F1.
```

## Comparação Entre os Paradigmas

O paradigma imperativo descreve de forma detalhada o passo a passo do algoritmo, enquanto o declarativo descreve a relação entre as variáveis e o sistema busca a solução automaticamente.

## Vantagens e Desvantagens

- **Imperativo**: Mais controle e eficiência, porém mais verboso e suscetível a erros.
- **Declarativo**: Código mais conciso e legível, ideal para sistemas baseados em regras, mas com menor controle de execução.

## Conclusão

O paradigma imperativo (Java) exige que o programador detalhe como o cálculo deve ser feito, controlando o fluxo e as operações.

Já o paradigma declarativo (Prolog) permite que o programador descreva apenas a lógica do problema, deixando a execução e a resolução para o interpretador.

Ambos alcançam o mesmo resultado, mas com abordagens conceituais diferentes, evidenciando a diversidade de estilos na programação.
