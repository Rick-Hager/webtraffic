# Brand Book — WebTraffic

> **Versão:** 1.0 — gerado pelo Consolidation Agent v1
> **Status:** Aguardando validação do cliente

---

## 1. Essência da Marca

A WebTraffic é uma agência de tráfego pago e marketing de performance que transforma cliques em clientes reais. A identidade visual deve comunicar **velocidade, precisão, confiança e crescimento** — os atributos que os clientes esperam de quem gerencia o dinheiro de mídia deles.

A marca posiciona-se como **consultiva e moderna**: técnica o suficiente para inspirar confiança em gestores exigentes, acessível o suficiente para nunca intimidar donos de PME que não dominam o jargão digital.

---

## 2. Logotipo

> **(decisão do consolidation)** — Nenhum arquivo de logo foi compartilhado pelo cliente. As diretrizes abaixo descrevem o sistema de marca proposto para validação.

### 2.1 Conceito
O logotipo da WebTraffic é wordmark com símbolo de acento gráfico. O símbolo representa **fluxo em movimento** — uma seta ou onda ascendente estilizada que remete ao crescimento de tráfego e à velocidade de resultados. O nome "WebTraffic" é escrito em caixa baixa com peso semibold para transmitir modernidade sem frieza excessiva.

### 2.2 Versões
| Versão | Uso |
|---|---|
| **Completa (símbolo + wordmark)** | Padrão — cabeçalhos, apresentações, materiais impressos |
| **Apenas símbolo** | Favicon, ícone de app, redes sociais em formato quadrado |
| **Apenas wordmark** | Rodapés, co-branding, espaços horizontais estreitos |
| **Monocromática escura** | Fundo branco ou claro |
| **Monocromática clara** | Fundo escuro ou colorido |

### 2.3 Área de proteção
O logotipo deve ter uma área de proteção mínima equivalente à altura da letra "W" em todos os lados. Nenhum outro elemento visual deve invadir essa área.

### 2.4 Proibições
- ❌ Não distorcer ou alterar proporções
- ❌ Não aplicar sombra ou contorno
- ❌ Não usar cores fora da paleta oficial
- ❌ Não rotacionar o logotipo
- ❌ Não aplicar sobre fundos que comprometam o contraste mínimo WCAG AA
- ❌ Não recriar o logotipo com outra fonte
- ❌ Não usar o nome "WebTraffic" separado do símbolo em materiais oficiais sem aprovação

---

## 3. Paleta de Cores

> **(decisão do consolidation)** — Paleta construída a partir do briefing de vertical (azul = confiança/tecnologia, laranja = energia/crescimento) e diferenciação de concorrentes. A confirmar com Rick Hager na validação.

### 3.1 Cores Primárias

| Nome | Hex | RGB | Uso |
|---|---|---|---|
| **Azul Principal** | `#1A56DB` | 26, 86, 219 | CTAs principais, links, destaques de dados |
| **Laranja Energia** | `#F97316` | 249, 115, 22 | CTAs secundários, badges, alertas positivos, acento gráfico |

### 3.2 Cores Neutras

| Nome | Hex | RGB | Uso |
|---|---|---|---|
| **Preto Profundo** | `#0F172A` | 15, 23, 42 | Textos principais, fundos dark |
| **Cinza Médio** | `#64748B` | 100, 116, 139 | Textos secundários, legendas, placeholders |
| **Cinza Claro** | `#E2E8F0` | 226, 232, 240 | Bordas, separadores, fundos sutis |
| **Fundo Off-white** | `#F8FAFC` | 248, 250, 252 | Fundo de seções alternadas |
| **Branco** | `#FFFFFF` | 255, 255, 255 | Fundo padrão, cards, formulários |

### 3.3 Cores de Sistema

| Nome | Hex | Uso |
|---|---|---|
| **Sucesso** | `#10B981` | Indicadores positivos, métricas verdes, checkmarks |
| **Atenção** | `#F59E0B` | Avisos, destaques intermediários |
| **Erro** | `#EF4444` | Erros de formulário, alertas críticos |
| **Info** | `#3B82F6` | Informativos, tooltips, notas |

### 3.4 Gradientes

| Nome | Código CSS | Uso |
|---|---|---|
| **Gradiente Principal** | `linear-gradient(135deg, #1A56DB 0%, #3B82F6 100%)` | Hero sections, banners de destaque |
| **Gradiente Energia** | `linear-gradient(135deg, #F97316 0%, #FB923C 100%)` | CTAs de alta prioridade, badges de oferta |
| **Gradiente Dark** | `linear-gradient(135deg, #0F172A 0%, #1E293B 100%)` | Fundos de seções escuras, rodapé |

---

## 4. Tipografia

> **(decisão do consolidation)** — Fonte **Inter** selecionada por ser moderna, altamente legível em telas, open-source (Google Fonts) e amplamente usada em produtos digitais B2B. A confirmar na validação.

### 4.1 Família Principal: Inter

```
@import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;500;600;700;800&display=swap');
```

| Peso | Nome | Uso |
|---|---|---|
| 400 (Regular) | Inter Regular | Corpo de texto, parágrafos, descrições |
| 500 (Medium) | Inter Medium | Labels, menus de navegação, botões secundários |
| 600 (SemiBold) | Inter SemiBold | Subtítulos, destaques inline, preços |
| 700 (Bold) | Inter Bold | Títulos de seção (H2, H3), botões principais |
| 800 (ExtraBold) | Inter ExtraBold | Títulos hero (H1), números de métricas |

### 4.2 Escala Tipográfica

| Token | Tamanho | Peso | Line-height | Uso |
|---|---|---|---|---|
| `text-hero` | 56px / 3.5rem | 800 | 1.15 | Título principal do hero |
| `text-h1` | 48px / 3rem | 800 | 1.2 | H1 de páginas internas |
| `text-h2` | 36px / 2.25rem | 700 | 1.25 | Títulos de seção |
| `text-h3` | 28px / 1.75rem | 700 | 1.3 | Sub-seções, títulos de cards |
| `text-h4` | 22px / 1.375rem | 600 | 1.35 | Títulos de items, acordeões |
| `text-lead` | 20px / 1.25rem | 400 | 1.6 | Parágrafo de introdução (lead) |
| `text-body` | 16px / 1rem | 400 | 1.7 | Corpo de texto padrão |
| `text-small` | 14px / 0.875rem | 400 | 1.5 | Legendas, notas, metadados |
| `text-xs` | 12px / 0.75rem | 500 | 1.4 | Badges, labels de tags |

### 4.3 Família Secundária
A WebTraffic usa apenas a família Inter em toda a comunicação digital para manter consistência e leveza no carregamento.

---

## 5. Tom Visual (Mood)

A identidade visual da WebTraffic deve evocar:

- **Profissionalismo moderno:** Limpo, organizado, com espaço em branco generoso
- **Precisão de dados:** Uso de números grandes, métricas destacadas, gráficos simples
- **Movimento e crescimento:** Elementos diagonais sutis, ícones de seta, gráficos ascendentes
- **Confiança técnica:** Sem excesso de decoração; funcionalidade que comunica competência
- **Energia positiva:** O laranja como ponto de acento traz calor e urgência sem comprometer a seriedade

**Referências visuais de mood:** Stripe, Linear, Vercel, HubSpot (interface) — design de produto SaaS orientado a dados.

---

## 6. Elementos Gráficos

### 6.1 Ícones
- **Biblioteca recomendada:** Lucide Icons (open-source, consistent stroke, SVG)
- **Estilo:** Linha (outline), stroke de 1.5px, cantos levemente arredondados
- **Tamanhos padrão:** 16px (inline), 20px (listas), 24px (destaques), 32px (seções), 48px (hero icons)
- **Cor:** Herda a cor do contexto (azul em seções claras, branco em seções escuras)
- ❌ Não misturar estilos de ícones (outline com filled)

### 6.2 Ilustrações e Gráficos
- Preferir **gráficos de dados reais** (barras, linhas ascendentes, funis) como elemento decorativo — reforçam a proposta de performance
- Quando necessário usar ilustração figurativa: estilo flat com cores da paleta oficial, traços limpos, sem sombra excessiva
- Imagens de pessoas: use preferencialmente fotos reais de clientes ou da equipe (nunca stock photos genéricos)

### 6.3 Formas e Padrões
- **Border radius padrão:** 8px (componentes), 12px (cards), 16px (containers maiores), 9999px (badges/pills)
- **Divisores:** Linha horizontal `1px solid #E2E8F0` ou espaçamento de seção
- **Background patterns sutis:** Grid de pontos ou linhas diagonais em tom sutil (`#E2E8F0` em fundo branco) em seções hero

---

## 7. Aplicações

### 7.1 Site
- **Fundo padrão:** Branco `#FFFFFF`
- **Seções alternadas:** Off-white `#F8FAFC`
- **Seções de destaque (CTA, hero de seção):** Gradiente dark ou azul principal
- **Texto sobre fundo escuro:** Branco `#FFFFFF` e `#CBD5E1`

### 7.2 Redes Sociais
- **Formato de post padrão:** Fundo escuro (`#0F172A`) com dados/números em destaque (branco + azul + laranja)
- **Stories/Reels:** Template com barra azul lateral, número grande de métrica central, texto de suporte
- **Avatar/Perfil:** Símbolo do logotipo em fundo azul `#1A56DB`
- **Capa LinkedIn/Facebook:** Fundo gradient dark com tagline e logo versão clara

### 7.3 Apresentações e Propostas
- **Slide de capa:** Gradient dark com logo branco e título do cliente
- **Slides de conteúdo:** Fundo branco, dados em azul, destaques em laranja
- **Tabelas de resultados:** Linha de header em azul `#1A56DB` com texto branco; alternância de linhas em branco / off-white
- **Fonte de apresentação:** Inter — mesma do site

### 7.4 Relatórios de Performance
- Números de métricas principais em `text-h2` + cor de contexto (verde para positivo, vermelho para negativo)
- Gráficos em cores da paleta oficial (azul = resultado atual, cinza = período anterior)
- Rodapé com logo WebTraffic + data + nome do cliente

---

*Fim do Brand Book v1.0*
