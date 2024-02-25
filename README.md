<!-- Título -->
# Entrada de Informações — O Comando “scanf()”

***Conteúdo da Aula:***

Para lermos as informações digitadas pelos usuários no console, precisamos utilizar o comando `scanf()` da biblioteca **stdio**.

A sintaxe (maneira de utilização do comando) do `scanf()` é basicamente ilustrada abaixo:

```C
scanf(<formato a ser lido>, <variável que receberá o valor lido>);
```

Perceba que nós precisamos passar o **“formato”** que deverá ser lido a partir do console.

É através deste formato, identificado com o `%`, é que o **C** sabe se o que será lido será um `int`, um `float` ou mesmo uma `string`, que para o **C** é um conjunto ou *array* de `char` (veremos o conceito de *arrays* adiante).

Abaixo, você pode verificar os formatos mais comuns:

| Formato | Descrição |
| :-----: | :-------: |
| `%c` | Sera lido um único caractere, devolvendo um char |
| `%s` | Sera lido um conjunto de caracteres ate que sejam pressionados a barra de espaço, tabulação ou enter. sera devolvido um *array* de `char` |
| `%d` | Leitura de um número, geralmente inteiro |
| `%f` | Leitura de um número, geralmente *float* |

Observe um exemplo de utilização do `scanf()`:

```C
#include <stdio.h>

void main() {
  char letra = ‘’;
scanf("%c", &letra);
// Enquanto o usuário não apertar ENTER, o console aguardará o usuário terminar a digitação.
// Quando ENTER for pressionado, o scanf() fará a leitura e transportará o valor lido para a variável apontada.

char nome[50]; // Um nome de até 50 caracteres.
scanf("%s", &nome);

int numero = 0;
scanf("%d", &numero);

float numeroQuebrado = 0;
scanf("%f", &numeroQuebrado);
}
```

Você deve ter reparado no `&` na frente das variáveis dentro do `scanf()`...

Isso na verdade indica para o **C** de que o valor lido do console deverá ser convertido e devidamente armazenado na mesma posição de memória que a variável indicada.

É sempre recomendável utilizar o operador `&` no `scanf()`, para garantir de que realmente o valor repassado pelo console será transportado para a variável.

<!-- Informações -->
## &#8505; Informações

![Visitors](https://api.visitorbadge.io/api/visitors?path=Devsgeeknerd%2Fcla-ent-inf-com-c-tra-com-ent-sai-dad-c-log-par-pro-com-bas&label=Visitantes&labelColor=%23700070&labelStyle=none&countColor=%23000fff&style=plastic&color=%23ffffff "Total de Visitantes")
&nbsp;
![Followers](https://img.shields.io/github/followers/Devsgeeknerd?style=p&label=Seguidores&labelColor=800080&color=000fff "Total de Seguidores")
&nbsp;
![Watchers](https://img.shields.io/github/watchers/Devsgeeknerd/cla-ent-inf-com-c-tra-com-ent-sai-dad-c-log-par-pro-com-bas?style=p&label=Observadores&labelColor=800080&color=000fff "Total de Observadores")
&nbsp;
![Stars](https://img.shields.io/github/stars/Devsgeeknerd/cla-ent-inf-com-c-tra-com-ent-sai-dad-c-log-par-pro-com-bas?style=p&label=Estrelas&labelColor=800080&color=000fff "Total de Estrelas")
&nbsp;
![Forks](https://img.shields.io/github/forks/Devsgeeknerd/cla-ent-inf-com-c-tra-com-ent-sai-dad-c-log-par-pro-com-bas?style=p&label=Bifurcações&labelColor=800080&color=000fff "Total de Bifurcações")
&nbsp;
![Repo Size](https://img.shields.io/github/repo-size/Devsgeeknerd/cla-ent-inf-com-c-tra-com-ent-sai-dad-c-log-par-pro-com-bas?style=p&label=Tamanho&labelColor=800080&color=000fff "Tamanho do Repositório")
&nbsp;
![License](https://img.shields.io/github/license/Devsgeeknerd/cla-ent-inf-com-c-tra-com-ent-sai-dad-c-log-par-pro-com-bas?style=p&label=Licença&labelColor=800080&color=000fff "Licença do Repositório")
