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
Abaixo são detalhados os achados da avaliação, organizados na síntese de problemas por tela e no mapeamento formal dos critérios WCAG violados.

## Síntese dos Problemas Encontrados

A tabela a seguir apresenta os problemas observados durante a inspeção, indicando o critério WCAG violado, a tela onde o problema ocorreu e a sua frequência de aparição no sistema.

| Problema | Critério WCAG | Tela/Página | Frequência |
| :--- | :--- | :--- | :---: |
| Seletores "Origem/Destino/Embarcações", "Ida e volta/Somente ida" inacessíveis via tecla Tab | 2.1.1 - Teclado /  | Origem/destino | 1 |
| Elementos ("Destino" e "Filtre por destinos populares / Saindo de") não acionam ao apertar Enter, a opção "Entre ou cadastre-se" é selecionada via teclado, mas exige o uso do mouse para prosseguir | 2.1.1 - Teclado / 4.1.2 - Nome, Função, Valor | Origem/destino | 1 |
| Tecla Espaço provoca a rolagem vertical da página em vez de acionar/selecionar elementos interativos focados | 2.1.1 - Teclado | Origem/destino | 1 |
| Obrigatoriedade de clique manual com mouse na janela modal de Cadastro/Login para que o foco do teclado comece a funcionar | 2.1.1 - Teclado / 2.4.3 - Ordem do Foco | Cadastro | 1 |
| Ícone de "visualizar senha" não é alcançável nem focável via tecla Tab | 2.1.1 - Teclado | Cadastro | 1 |
| Tecla Esc fecha toda a janela de cadastro ao ser acionada dentro de um submenu, gerando perda involuntária de dados | 2.1.1 - Teclado / 3.2.2 - Em Entrada | Cadastro | 1 |
| Tecla Esc não fecha painéis modais/overlays ("Detalhes da embarcação" e "Mais detalhes"), prendendo o foco ou exigindo mouse | 2.1.2 - Sem Armadilha de Foco | Seleção de passagens / Pagamento | 2 |
| Tecla Enter funciona para selecionar passagens, mas não aciona a seleção dos filtros de busca | 2.1.1 - Teclado | Seleção de passagens | 1 |
| Etapa indispensável de "Preencher dados dos passageiros" não é focável por teclado, exigindo clique com mouse para abrir | 2.1.1 - Teclado / 2.4.3 - Ordem do Foco | Pagamento | 1 |
| Leitor de tela (NVDA) percorre todo o conteúdo do fundo da página inicial antes de mover o foco para o modal de Login aberto | 2.4.3 - Ordem do Foco | Cadastro (Login) | 1 |
| NVDA não anuncia o rótulo/nome dos campos de e-mail, senha (login e cadastro) e documento (CPF/RG), lendo apenas "campo em branco" | 1.3.1 - Informação e Relações / 3.3.2 - Rótulos | Cadastro / Pagamento | 3 |
| Link "Cadastre-se" na janela de login é ignorado pela navegação por Tab no leitor de tela | 2.1.1 - Teclado | Cadastro | 1 |
| Botão de seleção de data (ida/volta) anunciado pelo NVDA sem a descrição de sua função de calendário | 4.1.2 - Nome, Função, Valor | Origem/destino | 1 |
| Leitura desordenada de campos e informações pelo NVDA, quebrando a sequência lógica de compreensão | 1.3.2 - Sequência Lógica | Origem/destino | 1 |
| Opções da seção "Forma de Pagamento" inacessíveis via Tab e não anunciadas pelo leitor de tela NVDA | 2.1.1 - Teclado / 4.1.2 - Nome, Função, Valor | Pagamento | 1 |
| Ícones de embarcações, tipos de acomodação (Rede, Camarote, Suíte) e logos de pagamento sem texto alternativo (`alt`) | 1.1.1 - Conteúdo Não Textual | Seleção de passagens / Pagamento | 2 |
| Cards de resultados de passagens construídos com blocos genéricos (`<div>`) em vez de listas organizadas (`<ul>`/`<li>`) | 1.3.1 - Informação e Relações | Seleção de passagens | 1 |
| Formulários de cadastro e pagamento sem etiquetas (`<label>`) vinculadas aos campos de digitação | 1.3.1 - Informação e Relações | Cadastro / Pagamento | 2 |
| Botão principal de confirmação de pagamento com texto claro sobre fundo claro, apresentando contraste insuficiente (< 4.5:1) | 1.4.3 - Contraste Mínimo | Pagamento | 1 |
| Ausência de contorno visual destacador (indicador de foco) ao navegar via Tab por campos de seleção de data, porto e pagamento | 2.4.7 - Foco Visível | Origem/destino / Pagamento | 2 |
| Instruções de formato correto e erros de validação (CPF/cartão) não vinculadas aos campos para leitura em tempo real | 3.3.2 - Rótulos ou Instruções | Pagamento | 1 |
| Botões de ação ("Cadastrar", "Destinos Populares", "Copiar PIX") construídos com `<div>` genéricas que não ativam via Enter/Espaço | 4.1.2 - Nome, Função, Valor | Cadastro / Pagamento / Origem/destino | 3 |
| Desalinhamento entre ícones e textos e distorção proporcional do ícone de passageiro ao aplicar Zoom de 200% | 1.4.4 - Redimensionar Texto | Origem/destino | 1 |

## Critérios WCAG violados

A tabela a seguir sumariza a relação de Princípios, Diretrizes e Critérios de Conformidade da WCAG 2.2 violados no sistema, com seus respectivos Níveis de conformidade.

| Princípio | Diretriz | Critério violado | Nível |
| :--- | :--- | :--- | :---: |
| **Perceptível** | 1.1 Alternativas em texto | 1.1.1 Conteúdo Não Textual | A |
| **Perceptível** | 1.3 Adaptável | 1.3.1 Informação e Relações | A |
| **Perceptível** | 1.3 Adaptável | 1.3.2 Sequência Lógica | A |
| **Perceptível** | 1.4 Distinguível | 1.4.3 Contraste Mínimo | AA |
| **Perceptível** | 1.4 Distinguível | 1.4.4 Redimensionar Texto | AA |
| **Perceptível** | 1.4 Distinguível | 1.4.12 Espaçamento de Texto | AA |
| **Operável** | 2.1 Acessível por Teclado | 2.1.1 Teclado | A |
| **Operável** | 2.1 Acessível por Teclado | 2.1.2 Sem Armadilha de Foco de Teclado | A |
| **Operável** | 2.4 Navegável | 2.4.3 Ordem do Foco | A |
| **Operável** | 2.4 Navegável | 2.4.7 Foco Visível | AA |
| **Compreensível** | 3.2 Previsível | 3.2.2 Em Entrada | A |
| **Compreensível** | 3.3 Assistência de Entrada | 3.3.2 Rótulos ou Instruções | A |
| **Robusto** | 4.1 Compatível | 4.1.2 Nome, Função, Valor | A |

## Considerações sobre os resultados

A avaliação realizada nas 4 telas do sistema Navegam evidenciou barreiras críticas de acessibilidade que impedem a utilização autônoma da plataforma por pessoas com deficiências visuais ou motoras:

1. **Dependência do Mouse:** Funções indispensáveis para a conclusão do fluxo (como dar o primeiro foco no modal de cadastro, abrir o preenchimento de dados do passageiro e escolher a forma de pagamento) exigem obrigatoriamente o uso do mouse.
2. **Navegação e Ordem de Foco:** O leitor de tela (NVDA) e a navegação por teclado encontram diversos pontos caindo em armadilhas de foco, perda de foco visível e ordens de leitura desordenadas que não seguem o fluxo visual da tela.
3. **Ausência de Semântica HTML:** O uso extensivo de elementos genéricos (`<div>`) para criar botões e cards sem atributos `aria-*` ou elementos semânticos apropriados (`<button>`, `<label>`, `<ul>`/`<li>`) impede leitores de tela de anunciar o papel, nome e valor dos componentes.
4. **Legibilidade e Design Visual:** Embora o sistema responda bem ao espaçamento de texto, o redimensionamento por zoom de 200% sofre com desalinhamentos visuais de ícones, e a tela de pagamento contém botões essenciais com taxa de contraste de cores inferior ao recomendado (4.5:1).

Recomenda-se a revisão semântica das telas, vinculação de rótulos aos campos de entrada, inclusão de suporte completo aos atalhos de teclado padrão (`Tab`, `Enter`, `Espaço`, `Esc`) e correção dos estilos de contraste e indicador de foco visível.


