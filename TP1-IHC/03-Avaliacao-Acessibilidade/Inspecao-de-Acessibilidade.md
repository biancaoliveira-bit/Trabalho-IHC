# Avaliação de Acessibilidade: Navegam

Esta seção apresenta a inspeção de acessibilidade realizada no sistema de transporte fluvial **Navegam** (`https://www.navegam.com.br/?origem=1&passageiros=1`), fundamentada na tradução oficial em português do Brasil das **Diretrizes de Acessibilidade para Conteúdo Web (WCAG 2.2)** do W3C. O objetivo desta avaliação é identificar barreira digitais que impeçam ou dificultem o acesso autonomous e equitativo de usuários com deficiências visuais, motoras, auditivas ou cognitivas.

---

## 1. Escopo da Avaliação

A inspeção cobriu o fluxo principal de consulta e compra de passagens no portal Navegam, englobando as seguintes telas e componentes críticos:

1. **Página Inicial / Formulário de Busca:** Filtros de seleção de cidade de origem, destino, data da viagem e quantidade de passageiros.
2. **Listagem de Viagens e Rotas Disponíveis:** Exibição dos cards de opções de embarcações, horários, preços e acomodações.
3. **Seleção de Acomodações e Assentos:** Modal/tela visual interativa para escolha das poltronas e suítes disponíveis na embarcação.
4. **Formulário de Identificação do Passageiro e Checkout:** Entrada de dados pessoais dos passageiros e etapa final de pagamento.

---

## 2. Processo Utilizado

A inspeção seguiu as etapas recomendadas para avaliação sistemática de acessibilidade baseada em heurísticas e diretrizes:

* **Detecção:** Análise individual e exploratória das páginas e componentes interativos utilizando navegação exclusiva por teclado (`Tab`, `Shift+Tab`, `Enter`, `Espaço`, setas direcionais) e leitores de tela, verificando estrutura semântica, contraste de cor e alternativas textuais.
* **Coleção:** Agrupamento e catalogação das falhas e barreiras encontradas durante a navegação, eliminando duplicatas entre fluxos semelhantes.
* **Discriminação:** Filtragem dos achados para separar defeitos de usabilidade geral de problemas reais de acessibilidade, associando cada falha observada ao seu respectivo Critério de Conformidade (WCAG 2.2) e grau de severidade.

---

## 3. Resultados da Inspeção

### 3.1. Síntese dos Problemas Encontrados

A tabela a seguir consolida os principais problemas de acessibilidade identificados no site Navegam, indicando o critério WCAG 2.2 violado, a localização da falha e sua frequência:

| Problema Encontrado | Critério WCAG 2.2 | Tela / Elemento | Frequência |
| :--- | :--- | :--- | :--- |
| Ícones e botões gráficos de navegação (como ícones de tipo de barco e calendário) sem descrição textual para leitores de tela | 1.1.1 Conteúdo Não Textual (Nível A) | Página Inicial / Listagem de Viagens | Alta (4) |
| Baixo contraste entre o texto cinza claro das informações secundárias (ex.: horários e trechos) e o fundo branco dos cards | 1.4.3 Contraste (Mínimo) (Nível AA) | Listagem de Viagens | Média (2) |
| O mapa interativo de seleção de poltronas não recebe foco via teclado, impedindo a escolha de assentos sem o uso do mouse | 2.1.1 Teclado (Nível A) | Seleção de Poltronas | Alta (1) |
| Ausência de indicação visual e textual clara de foco (`:focus`) em campos do formulário de busca e botões principais | 2.4.7 Foco Visível (Nível AA) | Página Inicial / Checkout | Alta (3) |
| Campos de entrada do formulário de dados do passageiro sem rótulos (`<label>`) explicitamente associados via código (`for`/`id`) | 3.3.2 Rótulos ou Instruções (Nível A) | Formulário de Checkout | Média (2) |
| Falta de estrutura hierárquica adequada de cabeçalhos (`<h1>`-`<h6>`), com seções utilizando apenas marcas em negrito (`<b>`) | 1.3.1 Informações e Relações (Nível A) | Listagem de Viagens | Alta (3) |

---

### 3.2. Critérios WCAG 2.2 Violados

A tabela abaixo correlaciona a estrutura formal dos Princípios e Diretrizes da WCAG 2.2 com os critérios específicos descumpridos pelo sistema:

| Princípio | Diretriz | Critério de Conformidade Violado | Nível |
| :--- | :--- | :--- | :--- |
| **1. Perceptível** | 1.1 Alternativas em Texto | **1.1.1 Conteúdo Não Textual** | A |
| **1. Perceptível** | 1.3 Adaptável | **1.3.1 Informações e Relações** | A |
| **1. Perceptível** | 1.4 Distinguível | **1.4.3 Contraste (Mínimo)** | AA |
| **2. Operável** | 2.1 Acessível por Teclado | **2.1.1 Teclado** | A |
| **2. Operável** | 2.4 Navegável | **2.4.7 Foco Visível** | AA |
| **3. Compreensível** | 3.3 Assistência de Entrada | **3.3.2 Rótulos ou Instruções** | A |

---

## 4. Considerações Gerais e Recomendações

A avaliação de acessibilidade realizada no portal **Navegam** evidenciou a existência de barreiras críticas de acessibilidade que afetam principalmente usuários que dependem da navegação por teclado e leitores de tela. 

### Principais Diagnósticos:
1. **Navegabilidade por Teclado:** A impossibilidade de interagir com o mapa visual de poltronas via teclado bloqueia a conclusão da compra para usuários com deficiência motora severa.
2. **Semântica e Leitores de Tela:** A falta de alternativas textuais em elementos gráficos e a carência de rótulos explícitos nos formulários prejudicam significativamente a navegação de usuários cegos ou com baixa visão.
3. **Legibilidade e Design Visual:** Os índices de contraste abaixo do recomendado exigem esforço visual excessivo para a leitura das condições da viagem.

### Recomendações de Melhoria:
* **Implementação de ARIA:** Incluir atributos como `aria-label` e `role="button"` em elementos interativos não nativos (como os assentos da embarcação).
* **Correção Semântica:** Associar adequadamente as tags `<label>` aos seus respectivos campos `<input>` no checkout e estruturar o conteúdo com cabeçalhos hierárquicos adequados (`<h1>`, `<h2>`).
* **Estilização de Foco e Contraste:** Adicionar indicadores visuais de foco bem definidos via CSS (`outline`) e readequar a paleta de cores para garantir a razão de contraste mínima de $4.5:1$ nos textos normais.
