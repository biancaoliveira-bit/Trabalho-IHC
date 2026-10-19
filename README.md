# Avaliação de Sistema - NAVEGAM

Trabalho Prático 1 (TP1) da disciplina **Interação Humano-Computador**.

**Instituição:** Universidade Federal do Amazonas (UFAM) - ICET  
**Professor:** Dr. Andrey Rodrigues

[Acessar a NAVEGAM](https://www.navegam.com.br/) · [Repositório do trabalho](https://github.com/biancaoliveira-bit/Trabalho-IHC) · [Navegar pelas etapas](#sumário-das-etapas)

## Visão geral

Este trabalho tem como objetivo avaliar o sistema NAVEGAM a partir de quatro perspectivas da Interação Humano-Computador: **usabilidade, experiência do usuário, acessibilidade e comunicabilidade**.

A proposta é identificar dificuldades de interação, compreender a percepção dos usuários e elaborar sugestões de melhoria fundamentadas nos métodos de avaliação estudados na disciplina. A documentação abrange o planejamento, a execução das avaliações, a análise dos resultados e os registros que apoiam a apresentação e a discussão do trabalho.

## Equipe

- Vanessa Coelho Pereira
- Manuely da Silva Simões
- Hisabelly Vasconcelos Alfaia
- Felipe Brandão de Souza
- Bianca Oliveira
- João Guilherme

## Sistema avaliado

A **NAVEGAM** é uma plataforma de busca e compra de passagens fluviais voltada a viagens pela Amazônia. Pelo site, os usuários podem pesquisar viagens informando origem, destino, datas e quantidade de passageiros, escolher entre somente ida ou ida e volta e consultar embarcações. O sistema facilita o planejamento de deslocamentos de barco e a compra de passagens pela internet.

[![Imagem de divulgação de passagens de lancha no site da NAVEGAM](https://www.navegam.com.br/assets/img/advertisements/comprarPassagemLancha.png)](https://www.navegam.com.br/)

*Imagem de divulgação disponibilizada no site oficial da NAVEGAM.*

O sistema pertence ao domínio de **serviços de viagens e transporte aquaviário**. O [documento de apresentação do sistema](TP1-IHC/00-Sistema/Apresentacao.md) é destinado ao detalhamento do público-alvo, das funcionalidades selecionadas e do escopo da avaliação.

Fontes da descrição: [página inicial da NAVEGAM](https://www.navegam.com.br/) e [Sobre nós](https://www.navegam.com.br/sobre-nos).

## Sumário das etapas

Os links abaixo permitem acessar os documentos de cada etapa do trabalho.

| Etapa | Documento | Conteúdo previsto |
| --- | --- | --- |
| Apresentação do sistema | [Apresentação da NAVEGAM](TP1-IHC/00-Sistema/Apresentacao.md) | Propósito, domínio, público-alvo, funcionalidades e escopo da avaliação. |
| Usabilidade: inspeção | [Inspeção de usabilidade](TP1-IHC/01-Avaliacao-Usabilidade/1-Inspecao.md) | Avaliação heurística, problemas identificados, severidade e sugestões de melhoria. |
| Usabilidade: teste | [Teste de usabilidade](TP1-IHC/01-Avaliacao-Usabilidade/2-Teste.md) | Planejamento, teste piloto, execução com participantes, evidências e análise dos resultados. |
| Usabilidade: Maze | [Documentação do Maze](TP1-IHC/01-Avaliacao-Usabilidade/3-Maze.md) | Configuração das tarefas e dos questionários, links e registros do teste na ferramenta. |
| Experiência do usuário | [Avaliação de UX](TP1-IHC/02-Avaliacao-UX/Experiencia-de-Uso.md) | Resultados do UEQ e análise qualitativa das respostas abertas no ATLAS.ti. |
| Acessibilidade | [Inspeção de acessibilidade](TP1-IHC/03-Avaliacao-Acessibilidade/Inspecao-de-Acessibilidade.md) | Escopo, verificações manuais e automatizadas e problemas relacionados à WCAG 2.2. |
| Comunicabilidade | [Avaliação pelo MAC](TP1-IHC/04-Avaliacao-Comunicabilidade/MAC,md) | Participantes, tarefas, registros das sessões e análise das rupturas de comunicabilidade. |

## Organização do repositório

Este README fica na raiz do repositório. Os documentos das etapas estão reunidos na pasta `TP1-IHC/`, conforme a organização atual apresentada abaixo.

| Local | Finalidade |
| --- | --- |
| `README.md` | Página inicial, visão geral e navegação pelo trabalho. |
| `TP1-IHC/00-Sistema/` | Apresentação do sistema e definição do escopo. |
| `TP1-IHC/01-Avaliacao-Usabilidade/` | Inspeção heurística, teste de usabilidade e documentação do Maze. |
| `TP1-IHC/02-Avaliacao-UX/` | Avaliação da experiência do usuário e análises quantitativa e qualitativa. |
| `TP1-IHC/03-Avaliacao-Acessibilidade/` | Inspeção e resultados de acessibilidade. |
| `TP1-IHC/04-Avaliacao-Comunicabilidade/` | Aplicação do MAC e registro das rupturas de comunicabilidade. |

<!-- Os links reproduzem os nomes existentes no repositório em 19/10/2026.
O enunciado, na página 3, exige a padronização dos diretórios e arquivos.
Ao adequar os nomes, atualizar também os links e a tabela deste README.
Em particular, o arquivo atual MAC,md deve ser corrigido para mac.md.
-->

## Resumo das avaliações

Esta versão apresenta os métodos previstos para o trabalho. Os resultados e as evidências de sua aplicação serão detalhados nos documentos de cada etapa conforme a documentação for concluída.

| Avaliação | Descrição |
| --- | --- |
| **Inspeção de usabilidade** | Aplicação da Avaliação Heurística com base nas heurísticas de Nielsen. O processo inclui exploração individual do sistema, reunião dos registros, identificação dos defeitos, classificação de severidade e propostas de melhoria. |
| **Teste de usabilidade** | Observação de participantes externos à equipe durante a realização de tarefas. Inclui planejamento, teste piloto e sessões oficiais, com registro de sucesso, dificuldades, erros e tempo de execução, apoiados pelo Maze. |
| **Experiência do usuário (UX)** | Aplicação do User Experience Questionnaire (UEQ) para analisar atratividade, perspicuidade, eficiência, confiabilidade, estimulação e novidade. A análise quantitativa é complementada pela codificação das respostas abertas e pela construção de redes no ATLAS.ti. |
| **Acessibilidade** | Inspeção orientada pela WCAG 2.2, com verificações de navegação por teclado, uso de leitor de tela, contraste, textos alternativos, estrutura do conteúdo, fonte e espaçamento. Os problemas devem ser relacionados aos critérios de acessibilidade correspondentes. |
| **Comunicabilidade** | Aplicação do Método de Avaliação de Comunicabilidade (MAC) para identificar momentos em que os usuários têm dificuldade de compreender a interface. As sessões são analisadas por meio da etiquetagem das rupturas, com registro dos trechos observados e consolidação dos resultados. |

## Ferramentas e instrumentos utilizados

| Recurso | Papel no trabalho |
| --- | --- |
| **Maze** | Organização das tarefas e dos questionários e apoio à coleta de dados do teste de usabilidade. |
| **UEQ** | Questionário e planilha de análise da experiência do usuário nas seis dimensões avaliadas. |
| **ATLAS.ti** | Análise qualitativa das respostas abertas, criação de códigos e construção de redes relacionadas às dimensões do UEQ. |
| **Notion** | Organização dos registros da inspeção de usabilidade e das etapas de detecção, coleção, discriminação e relato dos resultados. |
| **GitHub e Markdown** | Organização, versionamento e apresentação da documentação do trabalho. |

## Declaração de uso de IA

A equipe utilizou o **ChatGPT** como apoio à elaboração, à organização e à revisão textual deste README.md. A ferramenta foi utilizada como suporte à documentação. A revisão, a validação das informações e a responsabilidade pelo conteúdo entregue cabem integralmente aos integrantes da equipe.
