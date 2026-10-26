# Avaliação de Acessibilidade

Essa avaliação de acessibilidade foi feita no site da **Navegam** usando como guia as diretrizes da **WCAG 2.2** (Web Content Accessibility Guidelines). O objetivo aqui é encontrar o que está dificultando ou impedindo a navegação de pessoas com deficiência (seja visual, motora ou outra) e mostrar o que precisa ser ajustado no sistema.

---

## Escopo da avaliação

Para fazer os testes, a gente escolheu as telas e etapas mais importantes do fluxo de compra do site:

1. **Página Inicial:** Tela de busca onde o usuário escolhe origem, destino e quantidade de passageiros.
2. **Resultados da Busca / Listagem de Viagens:** Tela que mostra as opções de barcos, horários e preços disponíveis.
3. **Seleção de Assentos:** Etapa onde dá pra escolher a poltrona/acomodação na embarcação.
4. **Formulário do Passageiro / Checkout:** Tela para preencher os dados pessoais e confirmar o pedido.

---

## Processo utilizado

O processo seguiu a ideia de inspeção técnica e avaliação heurística, dividida em três fases principais:

* **Detecção:** Cada membro do grupo testou as telas de forma individual. A gente testou a navegação só usando o teclado (Tab, Enter, setas), checou se as imagens e ícones tinham texto alternativo, analisou o contraste das cores e a leitura das informações.
* **Coleção:** Juntamos todas as anotações e problemas encontrados por todo mundo em uma lista só, tirando as coisas repetidas.
* **Discriminação:** Analisamos a lista junta pra conferir se cada ponto era realmente um problema de acessibilidade ou se era alarme falso. Depois disso, definimos o nível de cada erro.

---

## Resultados da inspeção

### Síntese dos problemas encontrados

Abaixo estão os principais problemas de acessibilidade que a gente encontrou durante a navegação no site da Navegam:

| Problema | Critério WCAG | Tela/Página | Frequência |
| :--- | :--- | :--- | :--- |
| Ícones e botões de imagem sem texto alternativo explicando o que são | 1.1.1 Conteúdo não textual (Nível A) | Página Inicial / Listagem | 3 |
| Texto cinza claro sobre fundo branco com contraste ruim | 1.4.3 Contraste mínimo (Nível AA) | Listagem de Viagens | 2 |
| Dificuldade de selecionar o assento usando apenas o teclado | 2.1.1 Teclado (Nível A) | Seleção de Assentos | 1 |
| Campos de preenchimento sem aviso claro do que é obrigatório | 3.3.2 Rótulos ou Instruções (Nível A) | Formulário do Passageiro | 2 |
| Falta de organização nos títulos das seções (cabeçalhos HTML) | 1.3.1 Informações e Relações (Nível A) | Listagem de Viagens | 3 |

---

### Critérios WCAG violados

Organizando os problemas encontrados dentro das diretrizes e níveis da WCAG 2.2:

| Princípio | Diretriz | Critério violado | Nível |
| :--- | :--- | :--- | :--- |
| Perceptível | 1.1 Alternativas em texto | 1.1.1 Conteúdo não textual[cite: 21] | A |
| Perceptível | 1.3 Adaptável | 1.3.1 Informações e Relações[cite: 46] | A |
| Perceptível | 1.4 Distinguível | 1.4.3 Contraste mínimo[cite: 21] | AA |
| Operável | 2.1 Acessível por teclado | 2.1.1 Teclado[cite: 21] | A |
| Compreensível | 3.3 Assistência de Entrada | 3.3.2 Rótulos ou Instruções |  |

---

## Considerações sobre os resultados

Dá pra perceber que o site da Navegam resolve a parte básica da compra de passagens, mas deixa a desejar em acessibilidade. A maioria das falhas que encontramos está nos níveis **A** e **AA**, que são justamente os requisitos básicos e intermediários que todo site deveria cumprir.

A falta de descrição nos ícones atrapalha quem usa leitor de tela, e a dificuldade de navegar pelo teclado na hora de escolher a poltrona pode travar completamente a compra de quem tem limitação motora. Pra melhorar o site, vale a pena colocar etiquetas adequadas (tags e ARIA), ajustar o contraste das cores do texto e deixar a navegação pelo teclado mais fluida e visível.
