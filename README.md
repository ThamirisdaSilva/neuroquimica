# NeuroQuímica — Laboratório de avaliação e otimização de agentes de IA

Este Google Colab será utilizado como ambiente prático ao longo da disciplina **Otimizando Agentes de IA**.

Durante as aulas, vamos acompanhar a evolução do **NeuroQuímica**, um agente educacional criado para responder dúvidas sobre neurociência e química. A proposta é utilizar o mesmo agente durante toda a disciplina, passando pelas etapas de avaliação, diagnóstico, correção e melhoria contínua.

O Colab foi preparado para facilitar as atividades práticas. Grande parte da estrutura já está implementada para que você possa concentrar sua atenção na análise dos comportamentos do agente e nas decisões tomadas a partir das evidências encontradas.

---

## Como vamos trabalhar

A evolução do NeuroQuímica seguirá um ciclo:

**planejar → executar → avaliar → diagnosticar → corrigir → comparar → evoluir**

Cada aula produzirá um artefato que será utilizado nas etapas seguintes.

### Aula 1 — Planejando os testes

Você irá definir situações reais de uso do NeuroQuímica e transformar expectativas de qualidade em casos de teste.

Para cada caso, serão registrados elementos como:

* situação de uso;
* pergunta feita ao agente;
* comportamento esperado;
* critérios de avaliação;
* prioridade;
* justificativa.

Ao final, o Colab irá gerar:

`PLANO_TESTES_NEUROQUIMICA.csv`

Guarde esse arquivo. Ele será utilizado na Aula 2.

---

### Aula 2 — Construindo a baseline

Os casos definidos no plano de testes serão executados no NeuroQuímica.

Você irá registrar as respostas observadas e compará-las com os critérios definidos anteriormente.

Cada resultado será classificado e acompanhado de evidências que expliquem a decisão.

Ao final, será construída a primeira linha de base do agente:

`BASELINE_NEUROQUIMICA.csv`

Esse arquivo representa o comportamento atual do NeuroQuímica e servirá como referência para as próximas análises.

---

### Aula 3 — Diagnosticando as falhas

A partir das falhas prioritárias encontradas na baseline, vamos investigar possíveis causas.

A análise irá separar:

* sintoma;
* evidência;
* hipótese;
* causa provável.

Também serão realizadas pequenas verificações para fortalecer ou descartar hipóteses.

O resultado será uma **ficha de diagnóstico** para orientar as próximas intervenções.

---

### Aula 4 — Corrigindo e validando

Com base no diagnóstico, será realizada uma alteração controlada no agente.

Depois da mudança, vamos executar novamente:

* o caso que apresentou a falha;
* alguns casos que já funcionavam corretamente.

Os resultados serão comparados utilizando os mesmos critérios das avaliações anteriores.

Ao final, você deverá decidir se a alteração deve ser:

**mantida, ajustada ou revertida.**

---

### Aula 5 — Planejando a evolução

Na última etapa, reuniremos os aprendizados das aulas anteriores.

As falhas, evidências e oportunidades identificadas serão organizadas em um backlog de melhorias.

As ações serão priorizadas considerando:

* impacto;
* evidência;
* esforço;
* risco.

O resultado será o:

`PLANO_EVOLUCAO_NEUROQUIMICA`

Esse documento representará os próximos passos para a evolução do agente.

---

# Como utilizar este Colab

Execute as células na ordem em que aparecem.

Para executar uma célula, clique no botão **▶** localizado ao lado dela.

Algumas células exibem formulários interativos. Nesses casos, preencha os campos solicitados e utilize os botões disponíveis na própria interface.

Os dados adicionados serão exibidos abaixo do formulário para que você possa revisar sua atividade.

---

# Formulário do plano de testes

Na primeira atividade, você encontrará os seguintes campos:

**ID do Caso**

Identificador automático utilizado para acompanhar cada caso durante a disciplina.

Exemplo:

`T01`

**Tipo**

Representa o tipo de situação que está sendo testada.

Entre as opções disponíveis estão:

* dúvida conceitual;
* comparação;
* aplicação;
* pergunta ambígua;
* fora do escopo.

**Situação**

Descreva rapidamente o contexto em que o estudante está fazendo a pergunta.

Exemplo:

`Aluno revisando potencial de ação para uma prova.`

**Pergunta**

Digite exatamente aquilo que será enviado ao NeuroQuímica.

Exemplo:

`O que acontece durante a despolarização de um neurônio?`

**Comportamento esperado**

Descreva as principais características que uma resposta adequada deveria apresentar.

Exemplo:

`Explicar a abertura dos canais de sódio, a entrada de Na+ e a alteração do potencial da membrana utilizando linguagem adequada ao estudante.`

**Critérios**

Selecione os aspectos que serão utilizados para avaliar a resposta.

Você poderá utilizar critérios como:

* correção;
* clareza;
* atendimento ao pedido;
* adequação ao público;
* reconhecimento de limites.

**Prioridade**

Indique a importância daquele caso dentro da avaliação.

**Justificativa**

Explique brevemente por que aquele caso recebeu determinada prioridade.

---

# Botões disponíveis

### Adicionar caso

Inclui o caso preenchido no plano de testes.

Antes de adicionar, verifique se a pergunta, o comportamento esperado e os critérios foram preenchidos.

### Remover último caso

Remove o último caso adicionado.

### Limpar todos os casos

Apaga todos os casos registrados durante a execução atual.

Use essa opção com cuidado.

### Baixar plano de testes

Gera o arquivo:

`PLANO_TESTES_NEUROQUIMICA.csv`

O arquivo será utilizado nas próximas atividades da disciplina.

---

# Revisão do plano

Durante a atividade, o Colab também apresentará uma pequena revisão automática do conjunto de casos.

Ela poderá indicar situações como:

* ausência de casos de alta prioridade;
* pouca variedade entre os tipos de situação;
* quantidade reduzida de casos.

Esses avisos servem como apoio para revisar seu plano antes da exportação.

---

# Importante

Os arquivos produzidos durante as aulas fazem parte da evolução do NeuroQuímica.

Mantenha os arquivos gerados em cada etapa, pois eles serão utilizados como entrada para atividades posteriores.

Ao longo da disciplina, nosso objetivo será construir uma sequência de evidências que permita responder três perguntas:

**Como o agente está se comportando?**

**Por que determinados problemas estão acontecendo?**

**As mudanças realizadas realmente melhoraram o agente?**

Ao final, você terá acompanhado um ciclo completo de avaliação e evolução de um agente de IA.

