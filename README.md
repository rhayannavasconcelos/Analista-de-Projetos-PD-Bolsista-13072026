# Teste Prático I — Analista de Projetos P&D

Vaga: Analista de Projetos — P&D (Bolsista)

Duração máxima: 3 horas

## Introdução: Governança de Projetos em Geração Distribuída

Bem-vindo ao teste prático da Digital Grid! Você atua como **Analista de Projetos de P&D**. O time de Engenharia e Ciência de Dados recebeu duas bases (`consumer_unit_data.xlsx` e `power_plant_data.xlsx`) para criar um novo **"Motor de Rateio e Previsão de Consumo"**.

No Brasil, o crescimento da **Geração Distribuída (GD)** trouxe o **Sistema de Compensação de Energia Elétrica (SCEE)**. Nele, a energia excedente gerada por uma usina é injetada na rede e convertida em créditos para abater o consumo futuro de múltiplas Unidades Consumidoras (UCs). O grande desafio é o **rateio (alocação) desses créditos** de forma inteligente entre as UCs.

Antes dos Cientistas de Dados começarem a codificar, **você** precisa analisar o cenário, governar a qualidade dos dados e traduzir o desafio para a equipe técnica e para a diretoria. Este teste avalia sua capacidade analítica, sua lógica de negócio no setor elétrico e seu poder de síntese na comunicação.

---

## Recursos Fornecidos

Dois arquivos, na raiz deste repositório.

**`consumer_unit_data.xlsx`** — Histórico de consumo e saldo acumulado de créditos das UCs atreladas à usina.

**`power_plant_data.xlsx`** — Histórico de geração da Usina Teste.

Os dados são derivados de uma carteira real, anonimizados — **com os defeitos que dados de produção têm**. Não fizemos limpeza para você: as anomalias fazem parte do desafio.

---

## Notação

| Símbolo | Significado |
| --- | --- |
| `X` | Montante gerado pela usina no mês |
| `Y` | Consumo das UCs no mês |
| `Z` | Crédito acumulado na UC |
| `UC` | Unidade Consumidora |
| `SCEE` | Sistema de Compensação de Energia Elétrica |

---

## Entregável 1 — Auditoria Analítica e Matriz de Riscos

As bases brutas possuem anomalias. Explore os dados.

1. **Mapeie as 3 principais anomalias** presentes nas duas bases.
2. Crie uma **"Matriz de Risco"**, classificando a **Severidade** de cada anomalia (`Crítica`, `Moderada`, `Observação`) e justificando qual é o **impacto direto** no faturamento das UCs ou na regra de compensação, caso o Cientista de Dados treine o modelo com essa falha.
3. Descreva brevemente qual **instrução/regra** você passaria ao Cientista de Dados para tratar cada anomalia.

---

## Entregável 2 — Tradução Negócio-Tecnologia (Backlog Ágil)

O objetivo da próxima Sprint do time de P&D é criar a lógica de **"Rateio Otimizado de Créditos"**. Como a usina gera um montante `X`, as UCs consomem `Y` e têm crédito acumulado `Z`, precisamos distribuir a energia de forma inteligente.

1. Escreva de **2 a 4 User Stories** (Histórias de Usuário) claras, que traduzam o objetivo do negócio para a equipe de Ciência de Dados.
   *Formato:* **Como** [ator], **eu quero** [ação] **para que** [valor].
2. Inclua, em **pelo menos duas** User Stories, os **Critérios de Aceite** baseados nos dados.

---

## Entregável 3 — Relatório Executivo de Gestão

Analisando a curva histórica da `power_plant_data` vs. o total consumido na `consumer_unit_data`, percebe-se um comportamento de **tendência** ao longo dos meses.

Escreva um **comunicado (máx. 1 página)** direcionado à Diretoria da Digital Grid, contendo:

- Um **diagnóstico resumido** do balanço energético.
- Uma **recomendação de ação de negócios** para o próximo trimestre, com base nesses dados.

---

## Entregável 4 — Defesa Oral (Vídeo de até 5 minutos)

Você deve apresentar seu plano de ação na reunião de **"Sprint Planning"**. Grave um vídeo de **até 5 minutos** focado em:

- Qual foi a **anomalia de dados que mais te preocupou** e por quê.
- Como você **priorizou o Backlog Ágil** (Entregável 2) para garantir que os Cientistas de Dados entreguem o maior valor possível nas primeiras semanas.
- **Postura de dono(a)** do projeto.

---

## Entrega

### 1. Os documentos, num fork deste repositório

Faça um **fork** deste repositório (botão *Fork*, no topo da página), trabalhe nele e nos mande o link do seu fork. Não abra Pull Request — assim um candidato não vê a solução do outro.

O fork deve conter:

- **Entregável 1 — Auditoria e Matriz de Risco**: um documento (`.md` ou `.pdf`) com as 3 anomalias, a matriz de severidade/impacto e as instruções ao Cientista de Dados;
- **Entregável 2 — Backlog Ágil**: as User Stories e os Critérios de Aceite (`.md` ou `.pdf`);
- **Entregável 3 — Relatório Executivo**: o comunicado de até 1 página à Diretoria (`.md` ou `.pdf`);
- **o link do seu vídeo, no topo do `README.md` do fork** (veja o item 2).

Organize os arquivos de forma clara (uma pasta ou seção por entregável). Se usou alguma exploração de dados para embasar a auditoria, pode incluí-la — mas o foco é a **análise e a comunicação**, não o código.

### 2. Um vídeo de até 5 minutos, no YouTube

Grave o vídeo do **Entregável 4** (Defesa Oral), apresentando seu plano de ação como se fosse a reunião de Sprint Planning:

- A **anomalia de dados** que mais te preocupou e por quê.
- Como você **priorizou o Backlog Ágil** para entregar o maior valor nas primeiras semanas.
- **Postura de dono(a)** do projeto.

**Suba no YouTube como "Não listado"** (*Unlisted*) — não como "Privado", senão não conseguimos abrir. Não listado significa que só quem tem o link acessa; o vídeo não aparece em buscas nem no seu canal.

> No YouTube: **Enviar vídeo → Visibilidade → Não listado.**

**Cole o link no topo do `README.md` do seu fork**, assim:

```markdown
# Teste Analista de Projetos P&D — Digital Grid — <seu nome>

🎥 **Vídeo de apresentação:** https://youtu.be/xxxxxxxxxxx
```

### Para onde enviar

A entrega final do teste é feita **pelo formulário**:

**https://forms.gle/7NHo8SYNevCusue96**

Você só precisa do **link do seu fork**.

> **Precisando se comunicar durante o teste?** Escreva para **lucas@dg.energy**. Use esse e-mail.

---

## Como avaliamos

1. **Capacidade Analítica** — como você lida com dados ausentes ou inconsistentes e a solidez das suas métricas de avaliação. É o critério que mais pesa.
2. **Lógica de Negócios** — quão bem você traduziu o problema do setor elétrico (fórmulas e regras do SCEE) para sua análise.
3. **Comunicação** — clareza na classificação (Matriz de Risco), poder de síntese nos documentos e no vídeo executivo.

Boa sorte. Estamos ansiosos para ver sua solução.
