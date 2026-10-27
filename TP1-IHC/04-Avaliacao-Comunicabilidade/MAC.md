# Avaliação de Comunicabilidade

## Método utilizado
O Método de Avaliação de Comunicabilidade (MAC) é utilizado na área de Interação Humano-Computador (IHC) para avaliar se a interface de um sistema consegue se comunicar de forma clara com seus usuários.

Durante a interação, podem acontecer rupturas de comunicabilidade, que são momentos em que o usuário fica confuso, não entende como realizar uma ação ou não sabe como continuar utilizando o sistema. Essas situações são observadas e identificadas por meio de etiquetas, como “Cadê?”, “E agora?” e “Desisto”, que representam as dificuldades encontradas pelos participantes. A partir dessa análise, é possível entender quais partes da interface precisam ser melhoradas para tornar o sistema mais fácil de compreender e utilizar.

<div align="center">
<h4>  Etiquetas do MAC </h4>

| Etiqueta | Descrição |
|:---:|:---|
| Desisto | O usuário explicitamente admite não conseguir concluir uma tarefa. |
| Para mim está bom... | O usuário equivocadamente acredita que concluiu a tarefa. |
| Não, obrigado. | O usuário decide seguir por um caminho não preferido pelo designer, mesmo conhecendo o caminho preferido e sabendo como percorrê-lo.  |
| Vai de outro jeito. | O usuário não conhece, ou não consegue percorrer, o caminho de interação preferido pelo designer e então é obrigado a seguir outro caminho de interação. |
| Cadê? | O usuário não consegue expressar sua intenção através dos signos codificados na interface. |
| Ué, o que houve? | O usuário não percebe ou não compreende as respostas do sistema decorrente de uma ação anterior. |
| E agora? | O usuário não sabe o que fazer em determinado momento para concluir uma tarefa. |
| Onde estou? | O usuário tenta dizer algo que o sistema é capaz de entender em outro contexto, diferente do atual. |
| Epa! | O usuário cometeu um equívoco, percebe o engano e tenta desfazê-lo. |
| Assim não dá. | O usuário interrompe e abandona um caminho de interação com vários passos por considerá-lo improdutivo. |
| O que é isto? | O usuário não consegue interpretar o significado dos signos estáticos e dinâmicos codificados na interface. |
| Socorro! | O usuário consulta a ajuda online ou outras fontes de informação e explicação para concluir as tarefas. |
| Por que não funciona? | O usuário esperava obter determinados resultados do sistema e não entende por que o sistema produziu resultados diferentes do esperado. |

</div>

## Participantes e tarefas
### Participantes
+ Leano Guerreiro Baba
+ João Carlos Guimaraes Lannuzzi
### Tarefas
1. Definir se a viagem será somente de ida ou de ida e volta.
2. Informar a cidade de origem e a cidade de destino da viagem.
3. Definir a data de partida e, quando necessário, a data de retorno.
4. Informar a quantidade de passageiros que participarão da viagem.
5. Encontrar e escolher uma passagem de ida que atenda às necessidades da viagem.
6. Encontrar e escolher uma passagem de volta, caso a viagem seja de ida e volta.
7. Conferir as informações da viagem e o valor total antes de prosseguir com a compra.
8. Informar os dados pessoais necessários para realizar a compra.
9. Escolher uma forma de pagamento e fornecer as informações necessárias. só tem pix
10. Concluir a compra e verificar se a aquisição da passagem foi confirmada. só fica processando mas n processa

### Registro das sessões
- [Vídeo do participante Leano Guerreiro](https://youtu.be/DJKs1rXEuPQ?is=H8azo0JN1HbB79Xv)
- [Vídeo do participante João Carlos](https://youtu.be/JIPy1HMF4Yo?is=Y0gJD6PfsOga45vk)
  
## Etiquetagem das rupturas

| Part. | Tarefa | Tela/Elemento | Situação observada | Tipo de falha | Etiqueta | Problema de comunicabilidade |
|---|---|---|---|---|---|---|
| P01 | T2 | Selecionar o destino | "Não tem Recife" | Temporária | Epa! | Selecionou uma cidade que não correspondia no sistema  |
| P01 | T2 | Selecionar o destino | "Pode ser Belém" | Temporária | Vai de Outro jeito | Trocou a seleção para uma outra cidade buscando a conclusão da tarefa |
| P01 | T5 | Selecione a passagem de ida | "Não tem passagem" | Critica | Por que não funciona | Não encontra passagens disponiíveis, e o sistema não informa a falta de resposta |
| P01 | T5 | Inserir os dados de busca | "Tentar trocar alguma coisa" | Critica | E agora?  | O usuário tenta trocar os dados para vê se a uma mudança no retorno do sistema |
| P01 | T7 | Selecione a passagem de ida | "Não consegui realizar" | Critica | Desisto | O usuário desisti do seu objetivo final, por falta de retorno e direcionamento do sistema |
| P02 | T3 | Selecione a data | "não entendi se escolhi certo a data" | Temporária | O que é isto? | Há uma confusão na hora da escolha das datas |
| P02 | T6 | Seleção de passagem de volta | "agora quero escolher a passagem de volta | Temporária | Ué, o que houve? | O sistema atualiza para as informações da passagem, imposibilitando do usuário escolher sua passagem de volta |
| P02 | T6 | Informar os dados da busca | Usuário tenta fazer a busca | Temporária | Epa! | Usuário tenta buscar passagens sem informar a data, e o sistema retorna o erro |


## Consolidação das etiquetas

| Etiqueta | Ocorrências (P1) | Ocorrências (P2) | Total | Tarefas mais afetadas |
|---|---:|---:|---:|---|
| Desisto | 1 | 0 | 1 | T5 |
| Para mim está bom... | 0 | 0 | 0 | Nenhuma |
| Não, obrigado. | 0 | 0 | 0 | Nenhuma |
| Vai de outro jeito. | 0 | 0 | 0 | Nenhuma |
| Cadê? | 0 | 0 | 0 | Nenhuma |
| Ué, o que houve? | 0 | 1 | 1 | T6 |
| E agora? | 1 | 0 | 1 | T5 |
| Onde estou? | 0 | 0 | 0 | Nenhuma |
| Epa! | 1 | 1 | 2 | T2/T6 |
| Assim não dá. | 0 | 0 | 0 | Nenhuma |
| O que é isto? | 1 | 0 | 1 | T3 |
| Socorro! | 0 | 0 | 0 | Nenhuma |
| Por que não funciona? | 1 | 0 | 1 | T5 |

