# Estrutura do Site — WebTraffic

> **Versão:** 1.0 — gerado pelo Consolidation Agent v1
> **Status:** Aguardando validação do cliente

---

## 1. Hierarquia de URLs

```
/                          → Home
├── /servicos              → Página de Serviços
│   ├── #google-ads        → Âncora: Google Ads
│   ├── #meta-ads          → Âncora: Meta Ads
│   ├── #estrategia        → Âncora: Estratégia de Performance
│   └── #relatorios        → Âncora: Relatórios e BI
├── /sobre                 → Sobre a WebTraffic
└── /contato               → Formulário de Contato
    └── ?servico=<slug>    → Query param para pré-selecionar serviço no form
```

> **(decisão do consolidation)** — Estrutura minimalista de 4 páginas (Home, Serviços, Sobre, Contato). Adição de blog, cases ou páginas de nicho a avaliar com o cliente na validação.

---

## 2. Sitemap Detalhado

| URL | Tipo | Propósito | Prioridade SEO |
|---|---|---|---|
| `/` | Página | Apresentação geral, geração de leads | Alta |
| `/servicos` | Página | Detalhe dos serviços, conversão consultiva | Alta |
| `/sobre` | Página | Credibilidade, humanização da marca | Média |
| `/contato` | Página | Conversão direta — geração de lead | Alta |
| `/404` | Erro | Página de erro personalizada | — |

### Páginas futuras (fase 2 — a validar)

| URL | Tipo | Propósito |
|---|---|---|
| `/blog` | Listagem | SEO de conteúdo, autoridade |
| `/blog/[slug]` | Post | Artigo individual |
| `/cases` | Listagem | Prova social com cases reais |
| `/cases/[slug]` | Case | Case de sucesso individual |
| `/[nicho]` | Landing page | SEO local ou de nicho específico |

---

## 3. Menu Principal (Header)

### Desktop

```
[Logo WebTraffic]    Serviços    Sobre    Contato    [CTA: Análise gratuita]
```

| Item | Destino | Comportamento |
|---|---|---|
| Logo | `/` | Link sempre visível |
| Serviços | `/servicos` | Link direto |
| Sobre | `/sobre` | Link direto |
| Contato | `/contato` | Link direto |
| **CTA: Análise gratuita** | `/contato` | Botão primário (azul `#1A56DB`) |

### Mobile (Hamburger)

```
[Logo]                               [☰ Menu]
```

**Menu aberto (drawer lateral ou overlay):**
```
Serviços
Sobre
Contato
────────────────
[Análise gratuita]   ← CTA em destaque no fundo do menu
```

### Comportamento do Header

- **Sticky:** Header fixo no topo ao fazer scroll
- **Scroll-aware:** Fundo transparente no topo da home → fundo branco com sombra sutil após 80px de scroll
- **Estado ativo:** Item do menu correspondente à página atual recebe sublinhado ou cor de destaque

---

## 4. Footer

### Estrutura (4 colunas — Desktop)

```
┌─────────────────┬──────────────┬──────────────────┬─────────────────┐
│  [Logo]          │  Navegação   │  Serviços        │  Contato        │
│  WebTraffic      │  ─────────   │  ─────────────   │  ─────────────  │
│                  │  Serviços    │  Google Ads      │  WhatsApp       │
│  Tráfego pago    │  Sobre       │  Meta Ads        │  E-mail         │
│  que vira        │  Contato     │  Estratégia      │  Instagram      │
│  faturamento.    │              │  Relatórios      │  LinkedIn       │
└─────────────────┴──────────────┴──────────────────┴─────────────────┘
© 2025 WebTraffic. Todos os direitos reservados. | Política de Privacidade | CNPJ: [VALIDAR]
```

### Mobile (stacked)

```
[Logo + tagline]
[Links de navegação]
[Links de serviços]
[Informações de contato]
[Linha de rodapé]
```

---

## 5. CTAs Fixas e Flutuantes

### 5.1 CTA Sticky do Header
- **Texto:** `Análise gratuita`
- **Destino:** `/contato`
- **Visível em:** todas as páginas, sempre
- **Estilo:** Botão primário azul `#1A56DB`

### 5.2 Botão Flutuante de WhatsApp (opcional — a validar)
- **Posição:** Canto inferior direito, `fixed`, `z-index: 50`
- **Ícone:** WhatsApp verde
- **Destino:** `https://wa.me/[número — VALIDAR]?text=Olá! Vim pelo site da WebTraffic e gostaria de saber mais.`
- **Comportamento:** Aparece após 3 segundos de visita ou após 30% de scroll

### 5.3 Barra de CTA de Saída (Exit Intent — fase 2)
- Exibir modal suave quando o usuário move o cursor para fechar a aba (desktop)
- **Mensagem:** "Antes de ir — quer uma análise gratuita da sua conta de anúncios?"
- **CTA:** `Sim, quero` → `/contato`

---

## 6. Fluxo da Jornada do Visitante

### Jornada Principal: Descoberta → Lead

```
Busca no Google / Indicação / Redes Sociais
          │
          ▼
    [Home — /]
    ├── Lê headline (proposta de valor)
    ├── Vê métricas de prova social
    ├── Lê os 4 cards de serviços
    ├── Entende o processo ("Como funciona")
    ├── Vê diferenciais
    └── Clica no CTA
          │
          ▼
    [Contato — /contato]
    ├── Preenche formulário
    └── Submete → Mensagem de confirmação
          │
          ▼
    [Follow-up pela WebTraffic em até 24h]
    └── Ligação/WhatsApp → Reunião de diagnóstico gratuito
```

### Jornada Alternativa: Pesquisa de Serviço → Lead

```
Visitante chega pela Home
          │
          ▼
    Clica em "Ver todos os serviços"
          │
          ▼
    [Serviços — /servicos]
    ├── Lê detalhes do serviço específico
    ├── Vê o que está incluído
    └── Clica no CTA de serviço específico
          │
          ▼
    [Contato — /contato?servico=google-ads]
    └── Formulário pré-selecionado com o serviço escolhido
```

### Jornada de Credibilidade: Avaliação de Confiança

```
Lead quente (indicação ou retorno ao site)
          │
          ▼
    [Sobre — /sobre]
    ├── Lê a história e os valores
    ├── Conhece Rick Hager (equipe)
    └── Sente confiança para avançar
          │
          ▼
    [Contato — /contato]
```

---

## 7. Estrutura das Seções por Página

### Home (`/`)

```
01. Header (sticky)
02. Hero — H1 + Subtítulo + CTAs + texto auxiliar
03. Números / Métricas de prova social
04. Serviços — 4 cards
05. Como Funciona — 4 passos numerados
06. Diferenciais — 4 cards com ícone
07. Depoimentos — carrossel (ativar quando houver conteúdo real)
08. CTA final — bloco de conversão
09. Footer
```

### Serviços (`/servicos`)

```
01. Header (sticky)
02. Hero da página — H1 + Subtítulo
03. Google Ads — descrição + lista + CTA
04. Meta Ads — descrição + lista + CTA
05. Estratégia de Performance — descrição + lista + CTA
06. Relatórios e BI — descrição + lista + CTA
07. CTA final
08. Footer
```

### Sobre (`/sobre`)

```
01. Header (sticky)
02. Hero da página — H1 + Subtítulo
03. Nossa história — texto narrativo
04. Missão e valores — cards
05. Equipe — card de Rick Hager + demais (se houver)
06. CTA final
07. Footer
```

### Contato (`/contato`)

```
01. Header (sticky)
02. Hero da página — H1 + Subtítulo
03. Formulário de contato (coluna principal) + Informações de contato (coluna lateral)
04. Footer
```

---

## 8. Metadados e SEO Técnico

### Padrão de Title Tags

| Página | Formato |
|---|---|
| Home | `WebTraffic — [proposta de valor] | Google Ads e Meta Ads` |
| Serviços | `Serviços — WebTraffic | [serviço principal]` |
| Sobre | `Sobre a WebTraffic | [diferencial]` |
| Contato | `Fale com a WebTraffic | [benefício do contato]` |

### Open Graph (compartilhamento social)

- **og:image padrão:** 1200×630px — fundo escuro com logo e tagline
- **og:type:** website
- **og:locale:** pt_BR
- **Cada página** deve ter og:title e og:description únicos

### Robots e Indexação

- Todas as páginas: `index, follow`
- Formulário de sucesso (`/contato?enviado=true`): `noindex` (evitar indexação de página de confirmação)

### Canonical
- Cada URL tem canonical apontando para si mesma (evitar duplicate content)

---

*Fim do documento de Estrutura do Site v1.0*
