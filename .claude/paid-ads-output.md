# Koin App — Estratégia de Paid Ads: Meta Ads + Google UAC

---

## 1. Recomendação de Plataformas

### Plataforma primária: Meta Ads (Facebook + Instagram)

Meta is the primary recommendation for five structural reasons specific to Koin's audience:

**Alcance.** Classes C/D/E no Brasil são usuários intensos de Facebook e Instagram. Facebook mantém penetração alta em faixas de renda mais baixa e em regiões fora dos grandes centros. Instagram Reels cresce forte entre 25-45 anos nesse segmento.

**Targeting comportamental.** Meta permite segmentar por comportamentos financeiros (usuários sem cartão, usuários de Pix, compradores em Shopee/iFood/Mercado Livre), interesses de consumo, e dados demográficos cruzados com renda estimada. Nenhuma outra plataforma oferece esse nível de granularidade para esse público específico no Brasil.

**Mobile-first + App Events.** O produto é 100% app. Meta tem o melhor ecossistema de campanhas de App Installs com otimização para eventos pós-install como Activation (primeira compra). O algoritmo funciona muito melhor otimizando por Purchase do que por Install.

**Custo eficiente para o segmento.** CPMs em audiences de classes C/D/E no Brasil são significativamente menores que audiências premium.

**Benchmarks Brasil — fintechs/apps de crédito popular:**
- CPM: R$ 12–25 (feed), R$ 8–18 (Reels/Stories)
- CPC: R$ 1,80–4,50
- CPInstall: R$ 4–12 (varia por criativo e targeting)
- CPA Activation (referência de mercado): R$ 25–80 por usuário ativado

### Plataforma secundária: Google UAC (Universal App Campaigns)

Google captura intenção ativa que é complementar ao Meta. Usuários que pesquisam "parcelar sem cartão", "comprar parcelado pelo Pix", "app comprar sem cartão de crédito" têm intenção declarada. O CPInstall tende a ser maior, mas a taxa install → activation costuma compensar.

**Quando ativar:** Somente após Meta estabilizado e com 50+ eventos de Activation acumulados. Recomendação: ativar na semana 5-6, com 25-30% do budget total de mídia.

**Benchmarks Google UAC Brasil:** CPC Search R$ 3–9 para termos de crédito popular; CPInstall R$ 8–20.

**O que não priorizar agora:** TikTok (audiência 35-55 anos menor na plataforma — testar só após escalar Meta). LinkedIn e Twitter/X são irrelevantes para esse perfil de consumidor.

---

## 2. Estrutura de Campanha — Meta Ads

```
CONTA META ADS — KOIN APP
│
├── CAMPANHA 1: META_AppInstall_Prospecting_ColdAudience_BR_[MesAno]
│   Objetivo: App Installs → Otimizado para Activation (Purchase)
│   Orçamento: 50% do budget Meta
│   Bid strategy: Cost cap (manual → automated após 50 Activations)
│   Placements: Advantage+ (Feed, Reels, Stories, Audience Network)
│   │
│   ├── Ad Set 1: META_AS_Cold_Lookalike1pct_Ativados_BR
│   │   Audiência: Lookalike 1% baseado em evento Purchase (Activation)
│   │   Brasil nacional · Idade 20-55 · Todos os gêneros
│   │   Budget: 40% da campanha
│   │
│   ├── Ad Set 2: META_AS_Cold_Lookalike2-5pct_Ativados_BR
│   │   Audiência: Lookalike 2-5% baseado em Activation
│   │   Brasil nacional · Idade 20-55
│   │   Budget: 30% da campanha
│   │
│   └── Ad Set 3: META_AS_Cold_Interest_FinancasPopulares_BR
│       Audiência: Interest-based (detalhado na seção 4)
│       SP, RJ, BA, MG, DF, PR, RS · Idade 25-50
│       Budget: 30% da campanha
│
├── CAMPANHA 2: META_AppInstall_Retargeting_Warm_BR_[MesAno]
│   Objetivo: App Installs → Activation
│   Orçamento: 30% do budget Meta
│   │
│   ├── Ad Set 4: META_AS_Warm_Install_SemCompra_7d
│   │   Audiência: Instalaram nos últimos 7 dias, sem Purchase
│   │   Budget: 50% da campanha
│   │
│   ├── Ad Set 5: META_AS_Warm_Install_SemCompra_8-30d
│   │   Audiência: Instalaram há 8-30 dias, sem Purchase
│   │   Budget: 30% da campanha
│   │
│   └── Ad Set 6: META_AS_Warm_VideoViewers_50pct_30d
│       Audiência: Assistiram 50%+ dos vídeos de Koin nos últimos 30 dias
│       Budget: 20% da campanha
│
└── CAMPANHA 3: META_AppInstall_Testing_NewAngles_BR_[MesAno]
    Objetivo: App Installs → Activation
    Orçamento: 20% do budget Meta
    Finalidade: Testar novos ângulos criativos e audiences
    Regra: nunca cortar — é o motor de aprendizado
```

**Regras de escala:** Aguardar 7 dias e 50+ Activations antes de qualquer ajuste. Aumentar budget em máximo 20% por vez, intervalo mínimo de 3-5 dias. Nunca pausar campanha durante fase de aprendizado.

---

## 3. Ad Copy — 3 Variantes por Segmento (em Português)

### 3a. Cold Audience — Prospecting

**VARIANTE 1 — PAS (Problem-Agitate-Solve)**

Headline: Não tem cartão de crédito? Agora você pode parcelar do mesmo jeito.

Texto principal:
Quantas vezes você perdeu uma oportunidade de comprar algo que precisava porque não tinha cartão de crédito?

Sem limite, sem parcelamento, sem saída.

A Koin muda isso. Com o Pix Parcelado, você parcela suas compras em até 12x — sem cartão, sem burocracia. Tudo pelo Pix que você já usa. Shopee, iFood, Mercado Livre e muito mais.

Baixe agora e aproveite seu limite de crédito aprovado na hora.

CTA: Baixar agora

---

**VARIANTE 2 — BAB (Before-After-Bridge)**

Headline: Parcelar sem cartão. Isso agora existe.

Texto principal:
Antes: você via o produto que queria, via o preço parcelado, e ficava de fora porque não tinha cartão.

Depois: você abre a Koin, usa seu limite aprovado, e parcela pelo Pix. Ponto final.

A Koin é o app que te dá crédito pra comprar hoje e pagar no seu ritmo — sem precisar de cartão de crédito, sem filas, sem papelada.

Mais de [X] brasileiros já compraram assim.

CTA: Quero parcelar sem cartão

---

**VARIANTE 3 — Social Proof Lead**

Headline: Mais de [X] brasileiros já compraram parcelado sem cartão. Você pode ser o próximo.

Texto principal:
"Não acreditei quando vi que dava pra parcelar no Pix sem cartão." — Maria, São Paulo

Com a Koin, você baixa o app, tem seu limite aprovado em minutos e já pode parcelar nas suas lojas preferidas: Shopee, iFood, Mercado Livre, Amazon.

Sem cartão. Sem burocracia. Sem juros escondidos.

Seu próximo parcelamento começa aqui.

CTA: Baixar o app Koin

---

### 3b. Retargeting — Instalou mas Não Fez a Primeira Compra

**VARIANTE 1 — PAS (remoção de objeção)**

Headline: Você instalou a Koin. Falta só uma coisa.

Texto principal:
Você já está com a Koin no celular. Isso é o começo.

Mas se você ainda não fez sua primeira compra, talvez esteja com dúvida: "Fui aprovado? Onde eu uso? Como funciona?"

A resposta é simples: abre o app agora. Em menos de 5 minutos você vê seu limite, escolhe a loja e já faz seu primeiro pedido parcelado — no Pix, sem cartão.

Seu limite está esperando por você.

CTA: Abrir o app e comprar

---

**VARIANTE 2 — BAB (urgência + benefício tangível)**

Headline: Seu limite na Koin está disponível. Use antes de perder.

Texto principal:
Antes: sem cartão, sem parcelamento, sem opção.

Agora: você tem um limite aprovado na Koin esperando ser usado.

Depois: você compra o que precisa hoje, paga parcelado pelo Pix, e segue em frente.

Shopee, iFood, Mercado Livre, Amazon — tudo disponível agora no seu app Koin.

A primeira compra é a mais fácil. Bora?

CTA: Fazer minha primeira compra

---

**VARIANTE 3 — Social Proof Lead (redução de ansiedade)**

Headline: Quem usou a Koin pela primeira vez diz assim...

Texto principal:
"Fiquei com medo de não ser aprovado, mas foi fácil demais. Em 5 minutos já tava comprando na Shopee." — Carlos, MG

"Não sabia que podia parcelar pelo Pix. Agora não largo mais." — Fernanda, BA

Você já baixou o app. Agora é só dar o próximo passo: abrir, ver seu limite e fazer sua primeira compra parcelada.

Simples assim.

CTA: Ver meu limite agora

---

## 4. Especificação de Targeting de Audiência

### 4a. Cold — Interest-Based (Ad Set 3)

Localização: SP, RJ, MG, BA, DF, PR, RS | Idioma: PT-BR | Idade: 25-50 | Gênero: Todos

Camada 1 — Comportamentos financeiros (OR): usuários de Pix, compradores online frequentes, usuários de fintechs (Nubank, PicPay, Mercado Pago), interessados em crédito pessoal, empréstimo online, financiamento.

Camada 2 — Plataformas de compra (OR): Shopee Brasil, iFood, Mercado Livre, Amazon.com.br, Magazine Luiza.

Camada 3 — Refinamento socioeconômico: segmentos de menor renda disponíveis no Meta Brasil. Excluir interesses de classe AB (viagens internacionais, carros de luxo, etc.).

Tamanho por ad set: 5–15 milhões (evitar audiências estreitas demais).

### 4b. Lookalike Audiences (Ad Sets 1 e 2)

Base: apenas eventos de Activation (Purchase). Nunca usar todos os installs como base — o lookalike vai buscar usuários similares a quem comprou, não a quem só instalou. Atualizar a base mensalmente. Tamanho: 1% (similaridade máxima) e 2-5% (maior volume).

### 4c. Warm Audiences — Retargeting

| Evento | Janela | Ad Set |
|---|---|---|
| AppInstall sem Purchase | 1-7 dias | Ad Set 4 |
| AppInstall sem Purchase | 8-30 dias | Ad Set 5 |
| VideoView 50%+ | 30 dias | Ad Set 6 |
| Cadastro sem Purchase | 30 dias | Combinar com Ad Sets 4 e 5 |

### 4d. Exclusões Obrigatórias

| Exclusão | Motivo |
|---|---|
| Usuários com evento Purchase confirmado | Já ativados — CRM cuida deles, não paid |
| Usuários com 2+ compras | Retenção é de email/push/WhatsApp |
| Faixa etária abaixo de 20 anos | Fora do perfil-alvo |
| Interesses de classe AB (luxury, high-end travel) | Reduz desperdício de CPM |

Frequência máxima: cold = 2-3 impressões/semana; retargeting = 5-7 impressões/semana. Pausar criativos com frequência acima de 3,5 em cold audiences.

---

## 5. Checklist Pré-Lançamento — App Mobile

**SDK e Eventos**
- [ ] Meta SDK instalado no app (iOS e Android), versão atual
- [ ] Conversions API (CAPI) configurado no servidor — obrigatório para contornar iOS 14+
- [ ] Evento `AppInstall` disparando e verificável no Meta Events Manager
- [ ] Evento `CompleteRegistration` disparando no cadastro completo
- [ ] Evento customizado `CreditApproved` (limite aprovado) disparando corretamente
- [ ] Evento `Purchase` (primeira compra = Activation) disparando com valor correto
- [ ] Evento `Purchase` recorrente para segunda compra (usado nas exclusões)
- [ ] Todos os eventos testados com App Events Tester antes do go-live
- [ ] Janela de atribuição configurada: 7-day click, 1-day view
- [ ] Deduplicação entre SDK e CAPI configurada para evitar contagem dupla

**Links e UTMs**
- [ ] Deep link configurado para abrir tela correta do app (não a home da store)
- [ ] UTM parameters em todos os links
- [ ] Links App Store (iOS) e Google Play (Android) testados
- [ ] MMP configurado (AppsFlyer ou Branch.io) para atribuição multi-touch

**Compliance Financeiro — Brasil**
- [ ] Conta com categoria "Serviços Financeiros" ativada no Meta Business Manager
- [ ] Verificação de identidade da empresa concluída no Meta
- [ ] Copy revisado para conformidade com regras do Banco Central
- [ ] Criativos aprovados internamente pelo jurídico/compliance

**Configuração de Campanha**
- [ ] Evento de otimização configurado como `Purchase` (Activation) — não `AppInstall`
- [ ] Pelo menos 3 criativos por ad set ativos no lançamento
- [ ] Audiências de exclusão ativas antes do primeiro dia
- [ ] Alertas de CPA configurados

---

## 6. Brief Criativo — 2 Conceitos de Vídeo (15-30 segundos)

**Diretrizes gerais:**
- Formato vertical 9:16 para Reels/Stories; 1:1 para feed
- Closed caption obrigatória (85% assiste sem som)
- Aspecto UGC/nativo — produção polida performa pior para esse público
- Sem locução profissional — voz natural ou texto animado
- CTA na tela nos últimos 5 segundos

---

**CONCEITO 1: "A Cena do Carrinho"**

Ângulo: situação de constrangimento de não poder parcelar — identificação com a dor central.

- Hook (0-3s): Pessoa com expressão frustrada. Texto: "Queria parcelar mas não tem cartão?"
- Problema (3-8s): Sequência de situações: tenta comprar, vê "10x sem juros", não consegue. Texto: "Sem cartão, o parcelamento nunca foi pra você."
- Solução (8-20s): Screen recording: aprovação de limite, seleção de loja, "6x de R$XX no Pix", confirmação. Texto: "Com a Koin, você parcela pelo Pix. Sem cartão. Aprovação na hora."
- CTA (20-30s): "Baixe agora e parcele sem cartão." Icons App Store + Google Play.

Direção: gravar com celular, ambiente doméstico real. Persona: mulher 28-40 anos, classe C, nordeste ou sudeste. Duração ideal: 20-25s.

---

**CONCEITO 2: "Depoimento Real — Antes e Depois"**

Ângulo: prova social via UGC. Mais confiança que produção polida. Ideal para retargeting e cold.

- Hook (0-3s): "Eu não tinha cartão de crédito e achei que nunca ia poder parcelar."
- Problema (3-8s): "Toda vez que tentava comprar parcelado, sem cartão, não tinha como."
- Solução (8-20s): "Aí eu baixei a Koin. Me aprovaram na hora. Fui na Shopee, parcelei no Pix. Simples assim." + screen recording intercalado.
- CTA (20-30s): "Se você não tem cartão, baixa a Koin. Demora 5 minutos."

Direção: gravar com o próprio celular, zero edição pesada. Usar cliente real ou ator com perfil autêntico (25-45 anos, classe C/D). Testar versão SP vs. Nordeste para verificar impacto do sotaque regional. Duração ideal: 25-30s.

---

## 7. Ciclo de Vida Criativo e Fadiga

| Sinal de fadiga | Threshold | Ação |
|---|---|---|
| Frequência em cold audience | > 3,5 | Pausar criativo, introduzir novo |
| CTR caindo por 3 dias consecutivos | Queda > 20% da baseline | Testar novo hook |
| CPA subindo sem mudança de audience | Aumento > 30% por 5 dias | Refresh criativo completo |

Ciclo de vida esperado: 3-6 semanas em cold audiences. Manter sempre 2-3 criativos novos em pipeline.

**Hierarquia de testes:**
1. Conceito/ângulo (maior impacto)
2. Hook (primeiros 3 segundos)
3. Visual — UGC vs. screen recording vs. animação
4. Copy do corpo
5. CTA

---

## 8. Atribuição e CAC

Convenção de UTMs:
```
utm_source=meta
utm_medium=paid_social
utm_campaign=[objetivo]_[audiencia]_[mesano]
utm_content=[nome_do_adset]
utm_term=[id_do_criativo]
```

Modelo de atribuição: 7-day click, 1-day view. Comparar sempre Meta Ads Manager com MMP (AppsFlyer/Branch) — o Meta reporta números inflados. Usar o dado do MMP para decisões de budget.

**Cálculo de CAC correto:**
`CAC Activation = Spend total do canal / Usuários que fizeram a primeira compra atribuída ao canal`

Não usar Installs como denominador. O CAC por Activation é o que guia a otimização de budget.
