# Metodologia de Orçamentos — Roga Village · v2

**v2 (15/10/2026):** incorpora a base de orçamentos enviados de 15/08 a 14/10/2026
([`base/base-orcamentos-60d.md`](base/base-orcamentos-60d.md)).
**v1:** *Guia de Composição v2*, *Tabela de Preços — Roga* e *Modelo de Orçamento 0089/2026*.

Ferramenta: [`orcamento/index.html`](orcamento/index.html). As regras abaixo estão
implementadas nela, na aba **Checagens**.

> **Regra de ouro:** não vendemos uma sala, uma diária ou uma refeição. Vendemos uma
> experiência completa. A Tabela de Preços é a base. O orçamento é montado pela
> necessidade real do cliente, sem somar todos os itens da tabela.

---

## Passo a passo

| # | Etapa | O que fazer | Fonte |
|---|---|---|---|
| 1 | **Briefing** | Levantar: tipo e **objetivo** do evento · empresa e **quem decide** · datas candidatas · nº de pessoas (e se pode variar) · Day Use ou pernoite · horários · **exclusividade** · espaço fechado, aberto ou os dois · montagem · refeições · **restrição alimentar** · bebidas · banda/DJ/Happy Hour · rider · Team Building · **tempo para dinâmica** · **profissional ou A&B de fora** · **budget declarado**. | Guia §2 · Base §9 |
| 2 | **Budget** | Se o cliente disse um número, ele manda na composição. Montar dentro dele, ou mostrar o que sai do escopo. Orçamento muito acima do que o cliente precisava não volta. | Base §1, §9 |
| 3 | **Formato e horários** | Day Use: 08h às 22h. Pernoite: sala a partir das 08h, check-in às 15h e check-out às 13h. **Extensão de check-out = +50% da diária**, sujeita a disponibilidade. | Guia §5, §6 · Base §3 |
| 4 | **Hospedagem** | Diária **por Cubo** × nº de Cubos × diárias. **15 Cubos, até 4 pessoas por Cubo = 60 hóspedes no máximo.** Tabela Eventos tem ISS à parte; Tabela Lazer tem ISS embutido. A Diária Lazer é o único bloco em que tabela e prática estão sincronizadas, e **não varia**. | Tabela · Base §2.1, §3 |
| 5 | **Espaço** | Não cobrar duas vezes o mesmo uso. **Exclusividade = os 15 Cubos**, e aí não entra locação de espaço automática. Cozinha como adicional ao espaço foi cobrada a R$ 15.000 (prática). | Guia §4 · Base §2.6 |
| 6 | **Montagem** | Só 1 dia antes e só se houver disponibilidade operacional. Confirmar antes de prometer. | Guia §7 |
| 7 | **A&B** | Preço da tabela pela **duração** (1h, 2h ou 5h). A alimentação fatura no **mínimo 50 pessoas**; na duração de 5h, o mínimo é 100. Com restrição alimentar, incluir opção Wellness ou vegetariana. | Guia §8 |
| 8 | **A&B ou fornecedor de fora** | **Não existe política.** Qualquer pedido (ex.: oficina de pizza com insumos do fornecedor do cliente) vai à Gerência antes da resposta. | Base §8 |
| 9 | **Bebidas, banda, DJ** | Perguntar sempre. Banda ou DJ definem sonorização, palco e rider técnico-base. | Guia §9–§11 |
| 10 | **Experiências** | Team Building não é só locação de sala. **As experiências só existem dentro de evento:** não se vendem como day use avulso. Profissional de fora pode entrar, depois que a operação validar. | Guia §13, §14 · Base §2.5 |
| 11 | **Exceções** | Preço abaixo da tabela, desconto, mínimo reduzido, horário, montagem, experiência exclusiva, parcelamento e A&B de fora vão à **Gerência** antes de ir ao cliente. | Guia §16 |
| 12 | **Envio** | Na proposta: aviso de que não bloqueia sala/acomodação, 50% na confirmação, **parcelamento definido** e política de cancelamento. **Só usar preços da ferramenta, nunca material antigo** (caso R$ 5.120). | Modelo · Base §4, §7 |
| 13 | **Follow-up** | Registrar o desfecho (ganho ou perdido). Proposta enviada sem resposta há **mais de 10 dias** pede follow-up. | Base §1 |

## Fórmulas

```
Hospedagem   = Σ (diária × nº Cubos × diárias) + extensão de check-out (50% × diária × nº Cubos)
               + ISS sobre as diárias da Tabela Eventos
A&B          = Σ (valor p/ pessoa × máx(participantes, mínimo))
Serviços     = Σ (valor × qtd) + ISS sobre os itens marcados (no modelo, só a sala)
               — criança/adulto extra: qtd = pessoas × diárias
Experiências = Σ (valor p/ pax × pax)
TOTAL        = Hospedagem + A&B + Serviços + Experiências − desconto (com aprovação)
```

## Preços

### Diárias por Cubo

| Cubo | Evento c/ café | Evento pensão completa | Lazer c/ café | Lazer pensão completa |
|---|---|---|---|---|
| Individual | 750,00 | 975,00 | — | — |
| Duplo | 975,00 | 1.270,00 | 1.100,00 | 1.540,00 |
| Triplo | 1.265,00 | 1.650,00 | 1.320,00 | 1.848,00 |
| Quádruplo | 1.585,00 | 2.140,00 | 1.584,00 | 2.217,60 |

### Locação

Espaço sem cozinha R$ 26.000/diária · com cozinha R$ 34.000 · Sala de Eventos sem painel
R$ 8.500 · com painel de LED e operador R$ 10.500.

### Preços da prática (ainda fora da Tabela oficial)

Na ferramenta, estes itens aparecem com a marca *"prática — não oficial"*.

| Item | Valor | Origem |
|---|---|---|
| Extensão de check-out | +50% da diária | Texto-padrão de hospedagem, 28/09–09/10 |
| Cozinha como adicional ao espaço | R$ 15.000 | Orçamento de 03/09 (pela tabela seria R$ 8.000) |
| Adulto extra (por diária) | R$ 480 | Pacote de feriado de 7 de Setembro |
| Criança extra (por diária) | R$ 240 | Pacote de feriado de 7 de Setembro |
| Serviços avulsos e 9 experiências | ver catálogo | Modelo 0089/2026 |

---

## ⚠️ Pendências para a Gerência

| # | Ponto | Situação | Na ferramenta |
|---|---|---|---|
| 1 | **ISS** | A tabela diz 2% (eventos) e embutido (lazer); o orçamento real cobra 4%. | 2% na hospedagem e 4% nos serviços, editáveis. |
| 2 | **Sala de Eventos** | A tabela diz R$ 8.500/10.500; o modelo cobra R$ 15.000. | Usa a tabela. Avisa se o valor ficar abaixo, ou 50% acima. |
| 3 | **Cozinha adicional** | A tabela implica R$ 8.000; foi cobrado R$ 15.000. | R$ 15.000, marcado como prática. |
| 4 | **Parcelamento** | Convivem 3x (feriado), 5x (hospedagem) e 12x (Wellness Day). | O bloco "Formas de Pagamento" sai com *[a definir]* e só libera o envio sem alerta depois de editado. |
| 5 | **A&B de fora** | Não existe política e o cliente já perguntou. | Pergunta no briefing; se a resposta for sim, gera alerta. |
| 6 | **Horário das refeições** | Proposta de evento: café 08–09h, almoço 12–13h30, jantar 19h30–21h. Texto de hospedagem atual: café 08–10h, almoço 12–14h, jantar 20–22h. | Mantém o texto do modelo de evento. **Decidir qual vale.** |
| 7 | **Preços de hospedagem dispersos** | No mesmo mês saíram R$ 710, R$ 1.100, R$ 1.290, R$ 1.540 e R$ 1.960 de diária, por WhatsApp. | A Diária Lazer travada no valor da tabela gera alerta se for alterada. |
| 8 | **Oficializar** | Extensão de check-out, criança/adulto extra, "experiência só em evento" e cozinha a R$ 15.000 existem só na prática. | Já estão no catálogo, com a marca de prática. |
| 9 | **Pacote antigo R$ 5.120** | Continua gravado na oportunidade de Thiago Gentile Monaco no CRM. | Fora da ferramenta: **corrigir no CRM.** |

## Como atualizar preços

Edite o bloco `const TABELA = {...}` no início do `<script>` de `orcamento/index.html` e
publique o arquivo de novo. Os textos padrão ficam em `TEXTOS_PADRAO` e as perguntas do
briefing em `BRIEFING`. A pasta `base/` contém nomes de clientes e valores de pipeline:
**não publique essa pasta no site**, só o arquivo `orcamento/index.html`.
