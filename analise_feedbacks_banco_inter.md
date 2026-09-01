# 🎯 Desafio Criativo: Extraindo Insights do Feedback de Clientes Bancários

Este repositório contém a estrutura de um prompt avançado para análise de experiência do cliente (UX/CX) focado em aplicativos bancários, juntamente com a base de dados utilizada e os insights gerados pela IA.

**Nota sobre a origem dos dados:** As avaliações e comentários utilizados nesta análise são reais e foram coletados diretamente da página do aplicativo do **Banco Inter** na **App Store**.

## 1. O Prompt Estruturado

```text
Atue como analista de dados e experiência do cliente em um banco.
Sua tarefa é analisar feedbacks de clientes sobre aplicativo bancário, identificar temas recorrentes, sentimento dos clientes e oportunidades de melhoria.

Contexto: A análise será usada por uma equipe de experiência do cliente para priorizar melhorias nos canais digitais e reduzir atritos no atendimento. O foco é transformar comentários soltos em insights claros e acionáveis. Os dados analisados são referentes a avaliações reais de clientes do Banco Inter na App Store.

Dados disponíveis: Serão fornecidos comentários com data, canal de atendimento, texto do feedback, produto citado e nota de satisfação de 1 a 5.

Instruções de análise:
- Classifique os feedbacks por tema, sentimento, urgência e produto citado.
- Identifique os principais padrões, problemas, elogios e oportunidades.
- Aponte evidências nos dados fornecidos, usando exemplos curtos de comentários.
- Sugira ações práticas para a equipe de experiência do cliente e para o time responsável pelos canais digitais.

Formato da resposta: Entregue um resumo executivo com até 5 linhas, uma tabela com tema, sentimento, evidência e ação sugerida, além de uma lista final com as 3 prioridades mais importantes.

Restrições:
- Use apenas os dados fornecidos.
- Não invente números, causas ou conclusões.
- Não exponha dados pessoais ou sensíveis.
- Informe limitações quando os dados não forem suficientes.
- Use linguagem simples, direta e voltada para tomada de decisão.
```

## 2. Base de Dados (Avaliações Reais - Banco Inter na App Store)

| Data | Nota | Tema Principal | Texto do Comentário |
| :--- | :--- | :--- | :--- |
| 28/08/2026 | 5 | App / Inter Shop | "Uso o banco há anos e nunca tive problema. O app é super completo, a interface nova ficou boa e o Inter Shop salva muito com os cashbacks. Recomendo." |
| 29/08/2026 | 1 | Login / Estabilidade | "Depois da última atualização o app não abre de jeito nenhum. Fica na tela inicial carregando e fecha sozinho. Preciso pagar contas urgentes e não consigo acessar!" |
| 30/08/2026 | 3 | Usabilidade / UX | "O app tem muitas funções, o que é ótimo, mas acabou ficando muito poluído. É difícil achar coisas simples, como o extrato detalhado do mês anterior." |
| 30/08/2026 | 5 | Conta Global | "Conta global maravilhosa! Usei na minha viagem recente e funcionou perfeitamente. Câmbio justo e o cartão passou em todos os lugares." |
| 31/08/2026 | 2 | Atendimento | "O atendimento via chat é péssimo. A inteligência artificial (Babi) não entende o problema e demoro muito tempo para conseguir falar com um atendente humano." |
| 31/08/2026 | 4 | Cartão de Crédito | "Gosto muito das opções de investimento. Só acho que poderiam melhorar a área de cartões, a atualização do limite liberado demora a aparecer na tela." |
| 01/09/2026 | 1 | Pix | "Fiz um Pix, o dinheiro saiu da minha conta, mas não chegou no destino. O botão de gerar comprovante dá erro. Experiência frustrante." |
| 01/09/2026 | 5 | Taxas | "Interface do app tá cada vez melhor e mais intuitiva. Amo o fato de não ter taxas abusivas, resolve toda a minha vida financeira." |
| 01/09/2026 | 2 | Segurança / Jornada | "Muito chato ficar pedindo o i-safe (autenticador) toda hora, até para transações pequenas. Entendo que segurança é importante, mas quebra o fluxo e atrapalha o uso rápido." |
| 01/09/2026 | 3 | Pagamentos | "O banco é ok, mas o leitor de código de barras é horrível. A câmera quase nunca lê de primeira, sempre acabo tendo que digitar os números." |
| 01/09/2026 | 1 | Segurança | "Bloquearam minha conta preventivamente sem nenhum aviso! Tenho dinheiro lá, preciso pagar o aluguel e o suporte não me dá um prazo para resolver." |
| 01/09/2026 | 4 | Performance | "Ótimo banco, zero tarifas. A única reclamação é que a aba inicial tem tanta propaganda do shopping que o app fica meio pesado para carregar." |
| 01/09/2026 | 5 | Limite | "O aumento de limite no cartão de crédito pelo 'CDB Mais Limite' foi super rápido e fácil de fazer pelo celular. Funcionalidade excelente, a tela explica tudo." |
| 01/09/2026 | 2 | Estabilidade | "Toda vez que tem instabilidade eu fico na mão no caixa do mercado. Falta um aviso prévio ou uma notificação push avisando de manutenções no sistema." |
| 01/09/2026 | 4 | Navegação | "Uso como conta principal, gosto muito. Mas com as últimas atualizações, a navegação ficou um pouco confusa. Tem muitas abas e botões pequenos misturados." |

## 3. Insights Gerados pela IA

**Resumo Executivo**
A análise dos 15 feedbacks recentes revela que o app possui fortalezas notáveis em produtos como Conta Global e isenção de taxas (notas 5), mas sofre com atritos graves na jornada básica. Falhas críticas de estabilidade (app fechando após atualização), erros em transações Pix e ineficiência do bot de atendimento (Babi) geram forte urgência e notas 1. A usabilidade geral também é um ponto de atenção, com relatos de interface poluída e excesso de fricção por verificações de segurança.

**Tabela de Análise e Oportunidades**

| Tema | Sentimento | Evidência (Comentário) | Ação Sugerida |
| :--- | :--- | :--- | :--- |
| **Estabilidade e Login** | Negativo (Urgente) | *"app não abre de jeito nenhum. Fica na tela inicial... e fecha"* | Priorizar correção de bugs da última atualização; enviar patch emergencial. |
| **Atendimento (Chat)** | Negativo (Urgente) | *"A inteligência artificial (Babi) não entende... demoro muito tempo"* | Revisar árvore de decisão do bot e reduzir etapas para transbordo humano. |
| **UX e Navegação** | Misto / Negativo | *"muito poluído. É difícil achar coisas simples", "abas e botões misturados"* | Realizar testes de usabilidade para reestruturar a arquitetura de informação. |
| **Conta Global / Limite** | Positivo | *"Conta global maravilhosa!", "CDB Mais Limite foi super rápido"* | Manter a jornada fluida nestes produtos e usá-los como benchmark interno. |
| **Segurança (Autenticação)**| Negativo | *"Muito chato ficar pedindo o i-safe... até para transações pequenas"* | Ajustar o motor de risco para reduzir a fricção em transações habituais/baixo valor. |

**Top 3 Prioridades de Ação**
1. **Garantir o Acesso Básico:** Resolver imediatamente a instabilidade que impede o login e o fechamento inesperado do aplicativo.
2. **Otimizar a Resolução de Problemas:** Reduzir a barreira de atendimento do chat automatizado, garantindo acesso mais rápido a um atendente humano em casos urgentes.
3. **Limpeza Visual e Arquitetura de Informação:** Reduzir o excesso de anúncios na tela inicial e reorganizar menus para facilitar transações rápidas e consultas básicas (como extrato).
