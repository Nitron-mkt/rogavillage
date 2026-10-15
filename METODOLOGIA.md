# Metodologia de Orçamentos — Roga Village

Fontes: *Guia de Composição de Orçamentos v2*, *Tabela de Preços — Roga* e
*Modelo de Orçamento Eventos* (Proposta 0089/2026).
Ferramenta: [`orcamento/index.html`](orcamento/index.html). As regras abaixo estão
implementadas nela, na aba **Checagens**.

> **Regra de ouro:** não vendemos uma sala, uma diária ou uma refeição. Vendemos uma
> experiência completa. A Tabela de Preços é a base. O orçamento é montado pela
> necessidade real do cliente, sem somar todos os itens da tabela.

---

## Passo a passo

| # | Etapa | O que fazer | Guia |
|---|---|---|---|
| 1 | **Briefing** | Entender o evento antes de precificar: tipo e objetivo, nº de pessoas, Day Use ou pernoite, acomodações, espaços, horários, montagem antecipada, refeições, bebidas, banda/DJ, Happy Hour, rider técnico e Team Building. | §2 |
| 2 | **Formato e horários** | Day Use: 08h às 22h. Pernoite: sala a partir das 08h, check-in às 15h e check-out às 13h do dia seguinte. Horário diferente do padrão exige ajuste comercial. | §5, §6 |
| 3 | **Hospedagem** | Diária **por acomodação** = valor × nº de acomodações × diárias. Usar a Tabela Eventos (ISS à parte) ou a Tabela Lazer (ISS embutido). Conferir a capacidade: individual 1, duplo 2, triplo 3, quádruplo 4. | §3 |
| 4 | **Espaço** | Cobrar locação conforme o uso. **Não cobrar duas vezes o mesmo uso**: se o cliente loca todas as acomodações, a locação de espaço não entra automaticamente. Se loca a Sala de Eventos, não entra uma segunda locação pelo mesmo espaço. | §4 |
| 5 | **Montagem** | Só 1 dia antes e só se houver disponibilidade operacional. Confirmar com a operação antes de prometer ao cliente. | §7 |
| 6 | **A&B** | Preço por pessoa da tabela, conforme a **duração** (1h, 2h ou 5h). Na alimentação, faturar no mínimo **50 pessoas**. A tabela pode exigir mais: na duração de 5h, o mínimo é 100. | §8 |
| 7 | **Bebidas** | Perguntar sempre: pacote de bebidas, bebidas nas refeições, Happy Hour, confraternização e bar. | §9 |
| 8 | **Banda / DJ / técnica** | Perguntar sempre se haverá banda, DJ e Happy Hour. Com banda, dimensionar a estrutura a partir do **rider técnico-base**. Não escolher equipamento aleatoriamente. | §10, §11 |
| 9 | **Experiências** | Team Building, imersão, treinamento ou convenção não é só locação de sala: incluir Experiências Roga. Experiência personalizada só depois que a operação validar. | §13, §14 |
| 10 | **Exceções** | Preço abaixo da tabela, desconto, mínimo reduzido, mudança de horário, montagem antecipada e experiência exclusiva passam pela **Gerência** antes de ir ao cliente. | §16 |
| 11 | **Envio** | Na proposta: aviso de que o orçamento não bloqueia sala nem acomodações, condições (sinal de 50%) e política de cancelamento. | Modelo |

## Fórmulas (iguais às do modelo)

```
Hospedagem   = Σ (valor diária × nº acomodações × diárias) + ISS sobre as diárias da Tabela Eventos
A&B          = Σ (valor p/ pessoa × máx(participantes, mínimo))
Serviços     = Σ (valor × qtd/diárias) + ISS sobre os itens marcados (no modelo, só a sala)
Experiências = Σ (valor p/ pax × pax)
TOTAL        = Hospedagem + A&B + Serviços + Experiências − desconto (com aprovação)
```

## Tabela de diárias de hospedagem (valores calculados a partir das fórmulas da planilha)

| Cubo | Evento c/ café | Evento pensão completa | Lazer c/ café | Lazer pensão completa |
|---|---|---|---|---|
| Individual | 750,00 | 975,00 | — | — |
| Duplo | 975,00 | 1.270,00 | 1.100,00 | 1.540,00 |
| Triplo | 1.265,00 | 1.650,00 | 1.320,00 | 1.848,00 |
| Quádruplo | 1.585,00 | 2.140,00 | 1.584,00 | 2.217,60 |

Locação: espaço sem cozinha R$ 26.000/diária · com cozinha R$ 34.000 · Sala de Eventos
sem painel R$ 8.500 · com painel de LED e operador R$ 10.500.

---

## ⚠️ Divergências entre os documentos (a Gerência precisa decidir)

| # | Ponto | Tabela / Guia | Modelo 0089/2026 | Na ferramenta |
|---|---|---|---|---|
| 1 | **ISS** | Diária de evento: 2% à parte. Lazer: ISS embutido. | 4% na hospedagem e 4% na sala | Hospedagem 2% e serviços 4%, os dois editáveis em *Ajustes*. |
| 2 | **Sala de Eventos** | R$ 8.500 sem painel / R$ 10.500 com LED | R$ 15.000 | Catálogo usa a tabela. O vendedor pode subir o valor; se baixar, a ferramenta avisa. |
| 3 | **Mínimo de pessoas** | Tabela: 20 pax (1h), 50 (2h), 100 (5h). Guia: alimentação fatura mínimo de 50. | — | Alimentação: o maior entre 50 e o mínimo da duração. Bebidas: o mínimo da duração (20/50/100). |
| 4 | **Triplo c/ café (evento)** | R$ 1.265 | R$ 1.250 | Tabela. |
| 5 | **ISS nos outros serviços** | — | DJ, equipamentos e mesa de doces sem ISS | Marcação por item ("incide ISS"). Locação de espaço já vem marcada. |
| 6 | **Itens só do modelo** | Não estão na tabela | Mesa de doces, equipe de lazer, equipamentos, DJ, ambulância, salva-vidas e as 9 experiências | Entram no catálogo como "referência do modelo". Banda, rider, montagem e experiência personalizada ficam como *sob consulta*. |

**Recomendação:** colocar na Tabela de Preços oficial os serviços e as experiências que hoje
só aparecem no modelo, e fixar uma alíquota única de ISS. Assim a tabela continua sendo
a única fonte de preço.

---

## Como atualizar preços

Os preços ficam no bloco `const TABELA = {...}` no início do `<script>` de
`orcamento/index.html`. Para atualizar, edite os valores ali e publique o arquivo de novo.
Os textos padrão da proposta ficam em `TEXTOS_PADRAO`, e as perguntas do briefing em `BRIEFING`.
