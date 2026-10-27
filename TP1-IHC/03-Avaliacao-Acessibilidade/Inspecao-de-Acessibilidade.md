# Avaliação de Acessibilidade

Essa avaliação de acessibilidade foi feita no site da **Navegam**, usando como base as diretrizes da **WCAG 2.2**. O objetivo principal aqui é encontrar as barreiras digitais que dificultam ou barram o acesso de pessoas com deficiência (seja visual, motora ou outra) e mostrar o que precisa ser corrigido.

## Escopo da Avaliação

1. **Tela de Cadastro / Login**
2. **Tela Inicial (Origem/Destino)**
3. **Tela de Seleção de Passagens**
4. **Tela de Pagamento**

  Em cada uma das telas selecionadas, a avaliação cobriu **5 aspectos essenciais**:
* **Navegação por teclado:** Verificação de ordem de foco, operabilidade de botões/links (Tab, Enter, Espaço, Esc, Shift+Tab), armadilhas de foco e visibilidade do cursor de foco.
* **Leitor de tela:** Testes de navegação assistiva com o software NVDA para checar a leitura de rótulos, avisos de instrução, anúncios de componentes interativos e sequência lógica de leitura.
* **Contraste de cores:** Análise da relação de contraste visual entre texto e fundo em botões e elementos interativos essenciais.
* **Legibilidade dos textos:** Testes de redimensionamento do texto com zoom de 200% do navegador e aplicação de ferramentas de espaçamento personalizado (Text Spacing) sem perda de funcionalidade.
* **Imagens e textos alternativos:** Inspeção de ícones decorativos e informativos (embarcações, acomodações, métodos de pagamento) quanto à presença de atributos adequados.

## Processo Utilizado

A equipe seguiu um fluxo de inspeção em três etapas:

1. **Detecção:** Testes individuais com teclado, leitor de tela NVDA, contraste e zoom de 200%.
2. **Coleção:** Registro sistemático de cada falha, barreira de acesso e comportamento inconsistente observado em relação a cada um dos 5 aspectos avaliados nas 4 telas.
3. **Discriminação:** Agrupamento e classificação dos problemas encontrados, relacionando cada achado diretamente aos Princípios, Diretrizes e Critérios de Conformidade da WCAG 2.2.

## Resultados da inspeção

## Síntese dos Problemas Encontrados
Abaixo são detalhados os achados da avaliação, organizados na síntese de problemas por tela e no mapeamento formal dos critérios WCAG violados.

| Problema Identificado | Critério WCAG | Tela / Página | Freq. |
| --- | --- | --- | ---: |
| Ausência de texto alternativo (`alt`) em ícones essenciais | 1.1.1 Conteúdo Não Textual | Inicial / Passagens | 5 |
| Formulários de login, cadastro e pagamento sem etiquetas (`label`) | 1.3.1 Info e Relações / 3.3.2 | Login / Pagamento | 4 |
| Cards de passagens construídos em `<div>` genéricos sem listas | 1.3.1 Informação e Relações | Seleção Passagens | 1 |
| Contraste insuficiente no botão principal de pagamento | 1.4.3 Contraste Mínimo | Tela de Pagamento | 1 |
| Seletores de origem/destino e pagamento ignorados pelo Tab | 2.1.1 Teclado | Inicial / Pagamento | 3 |
| Uso obrigatório de mouse para focar o modal de cadastro | 2.1.1 Teclado | Login / Cadastro | 3 |
| Tecla Esc não fecha modais ou fecha a janela inteira por engano | 2.1.2 Sem Armadilha de Foco | Cadastro / Passagens | 2 |
| Salto da ordem lógica de foco ao abrir modais ou usar filtros | 2.4.3 Ordem do Foco | Login / Passagens | 2 |
| Remoção do contorno visual de foco (`outline`) nos campos | 2.4.7 Foco Visível | Geral (Formulários) | 4 |
| Botões genéricos em `<div>` que não acionam com Enter/Espaço | 4.1.2 Nome, Função, Valor | Inicial / Pagamento | 3 |

## Critérios WCAG violados

| Princípio | Diretriz | Critério Violado | Nível |
| --- | --- | --- | --- |
| Perceptível | 1.1 Alternativas em Texto | 1.1.1 Conteúdo Não Textual | Nível A |
| Perceptível | 1.3 Adaptável | 1.3.1 Informação e Relações | Nível A |
| Perceptível | 1.4 Distinguível | 1.4.3 Contraste (Mínimo) | Nível AA |
| Operável | 2.1 Acessível por Teclado | 2.1.1 Teclado | Nível A |
| Operável | 2.1 Acessível por Teclado | 2.1.2 Sem Armadilha de Foco de Teclado | Nível A |
| Operável | 2.4 Navegável | 2.4.3 Ordem do Foco | Nível A |
| Operável | 2.4 Navegável | 2.4.7 Foco Visível | Nível AA |
| Compreensível | 3.3 Assistência Entrada | 3.3.2 Rótulos ou Instruções | Nível A |
| Robusto | 4.1 Compatível | 4.1.2 Nome, Função, Valor | Nível A |

## Considerações sobre os resultados
