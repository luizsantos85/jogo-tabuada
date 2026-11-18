# 🧮 Jogo da Tabuada

Jogo simples para praticar a tabuada do **2 ao 12**, feito com [Vue 3](https://vuejs.org/) em um único arquivo HTML.

👉 **Jogar online:** https://luizsantos85.github.io/jogo-tabuada/

## Como funciona

- A cada partida são sorteadas **12 contas** diferentes (tabuada do 2 ao 12, multiplicando de 1 a 10).
- Cada conta tem **15 segundos** para ser respondida.
- Se o tempo acabar, a conta é pulada e **volta no final** para uma segunda chance.
- Se o tempo acabar de novo, ela conta como erro.
- No final aparece o **placar de acertos e erros** e uma revisão das contas erradas com a resposta certa.

## Rodando localmente

Não precisa instalar nada: basta abrir o `index.html` no navegador.

Para acessar de outro aparelho na mesma rede, sirva a pasta com qualquer servidor estático, por exemplo:

```bash
python3 -m http.server 8080
```

## Personalizando

No `index.html`, dentro de `data()`:

| Opção   | Padrão | O que faz                     |
|---------|--------|-------------------------------|
| `TOTAL` | `12`   | Quantidade de contas por jogo |
| `TEMPO` | `15`   | Segundos para cada conta      |

Para mudar quais tabuadas entram no sorteio, ajuste os laços em `gerarPerguntas()`.

## Tecnologias

- Vue 3 (via CDN)
- HTML + CSS puro
