# ⛽ Etanol ou Gasolina?

App simples e rápido para decidir na bomba: **vale a pena abastecer com etanol ou com gasolina?**

## Como funciona

Você digita o preço de **um** dos combustíveis — etanol ou gasolina, alternando no seletor — e o app mostra o **preço-limite** do outro. É só comparar com o valor da bomba:

**Modo etanol** (padrão): mostra até quanto a **gasolina compensa**.
- 🟢 Gasolina **mais cara** que o valor mostrado → abasteça com **ETANOL**
- 🔴 Gasolina **mais barata** → abasteça com **GASOLINA**

**Modo gasolina**: mostra até quanto o **etanol compensa**.
- 🟢 Etanol **mais barato** que o valor mostrado → abasteça com **ETANOL**
- 🔴 Etanol **mais caro** → abasteça com **GASOLINA**

O último preço de cada modo e a última aba usada ficam salvos no aparelho.

### Exemplo

Etanol a **R$ 3,50** → o app mostra **R$ 5,00** ("Gasolina compensa até").
Se a gasolina estiver acima de R$ 5,00, o etanol compensa.

Gasolina a **R$ 5,00** → o app mostra **R$ 3,50** ("Etanol compensa até").
Se o etanol estiver abaixo de R$ 3,50, compensa abastecer com ele.

## A regra dos 70%

Motores flex consomem cerca de 30% mais etanol do que gasolina para a mesma distância. Por isso, o etanol só vale a pena quando custa **até 70% do preço da gasolina**:

```
preço do etanol ≤ 0,70 × preço da gasolina  →  etanol compensa
```

Ou, de forma equivalente: o etanol compensa quando a gasolina custa **mais que** `(preço do etanol) ÷ 0,70`.

> 💡 Motores flex mais recentes têm rendimento melhor com etanol. Se o seu for assim, você pode ajustar o percentual (ex.: 73%) em **Ajustes avançados** — a escolha fica salva no aparelho.

## Como usar no posto

1. Abra o app (funciona offline, direto do celular).
2. Escolha Etanol ou Gasolina e digite o preço visto na bomba.
3. Compare o valor-limite mostrado com o preço do outro combustível — e abasteça.

## Instalar no celular (PWA)

O site é um **Progressive Web App**: pode ser instalado como um app comum, sem loja de aplicativos.

- **Android (Chrome):** abra o site → menu ⋮ → *"Adicionar à tela inicial"*.
- **iPhone (Safari):** abra o site → botão *Compartilhar* → *"Adicionar à Tela de Início"*.

O último preço digitado e o percentual escolhido ficam salvos no aparelho.

## Tecnologias

- HTML + CSS + JavaScript puro (sem dependências)
- PWA com manifest e service worker
- Funciona offline

## Licença

Uso livre para fins pessoais.
