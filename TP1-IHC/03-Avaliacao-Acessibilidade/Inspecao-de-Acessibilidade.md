# Avaliação de Acessibilidade

Essa avaliação de acessibilidade foi feita no site da **Navegam**, usando como base as diretrizes da **WCAG 2.2**. O objetivo principal aqui é encontrar as barreiras digitais que dificultam ou barram o acesso de pessoas com deficiência (seja visual, motora ou outra) e mostrar o que precisa ser corrigido.

## Escopo da avaliação
Para fazer a inspeção, a gente olhou bem para as telas e fluxos mais importantes do site:
1. **Página Inicial:** Tela de busca de origem e destino das viagens fluviais.
2. **Listagem de Viagens:** Tela que mostra os barcos, horários e rotas disponíveis.
3. **Seleção de Assentos:** Etapa onde o usuário escolhe o lugar a bordo.
4. **Formulário do Passageiro / Checkout:** Parte de preenchimento de dados e fechamento da compra.

---

## Processo utilizado
O trabalho seguiu o método de inspeção e avaliação passo a passo:
* **Detecção:** Cada integrante do grupo testou o site de forma independente, verificando a navegação só pelo teclado, a falta de textos alternativos em imagens, o contraste das cores e a leitura por recursos de acessibilidade.
* **Coleção:** Juntamos todos os achados em uma única lista e tiramos o que estava repetido.
* **Discriminação:** Analisamos os pontos para separar o que é defeito real de acessibilidade do que era falso positivo.

---

## Resultados da inspeção

### Síntese dos problemas encontrados
A tabela abaixo resume os principais problemas achados nas páginas da Navegam:

| Problema | Critério WCAG | Tela/Página | Frequência |
| :--- | :--- | :--- | :--- |
| Ícones e botões de imagem sem texto alternativo descritivo | 1.1.1 Conteúdo não textual (Nível A) | Página Inicial / Listagem | 3 |
| Texto cinza claro sobre o fundo branco com contraste ruim | 1.4.3 Contraste mínimo (Nível AA) | Listagem de Viagens | 2 |
| Dificuldade para mexer e selecionar assentos usando só o teclado | 2.1.1 Teclado (Nível A) | Seleção de Poltronas | 1 |
| Campos de preenchimento obrigatório sem aviso claro | 3.3.2 Rótulos ou Instruções (Nível A) | Formulário de Identificação | 2 |
| Falta de organização correta nos cabeçalhos das seções | 1.3.1 Informações e Relações (Nível A) | Listagem de Viagens | 3 |

### Critérios WCAG violados
Aqui está o resumo dos princípios e critérios que o site acabou violando:

| Princípio | Diretriz | Critério violado | Nível |
| :--- | :--- | :--- | :--- |
| Perceptível | 1.1 Alternativas em texto | 1.1.1 Conteúdo não textual | A |
| Perceptível | 1.3 Adaptável | 1.3.1 Informações e Relações | A |
| Perceptível | 1.4 Distinguível | 1.4.3 Contraste mínimo | AA |
| Operável | 2.1 Acessível por teclado | 2.1.1 Teclado | A |
| Compreensível | 3.3 Assistência de Entrada | 3.3.2 Rótulos ou Instruções | A |

---

## Considerações sobre os resultados
Dá para ver que o site da Navegam até funciona para o básico, mas peca bastante em acessibilidade. A maioria dos erros está nos níveis **A** e **AA**, que são justamente os requisitos básicos que todo sistema digital deveria respeitar. 

A falta de descrição nos ícones atrapalha quem usa leitor de tela, e o problema no teclado para escolher os assentos trava quem tem dificuldade motora. A recomendação principal é ajustar as tags e o contraste para deixar o site inclusivo para todo mundo.
