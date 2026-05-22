# Design Guidelines — WebTraffic

> **Versão:** 1.0 — gerado pelo Consolidation Agent v1
> **Status:** Aguardando validação do cliente

> Os tokens abaixo devem ser implementados como CSS Custom Properties na raiz do projeto Astro (`src/styles/global.css` ou equivalente). Eles espelham com fidelidade a paleta e a tipografia definidas no `brand-book.md`.

---

## 1. Design Tokens CSS

### 1.1 Cores

```css
:root {
  /* ─── Cores Primárias ─────────────────────────────────────────── */
  --color-primary:          #1A56DB;  /* Azul principal — CTAs, links, destaques */
  --color-primary-hover:    #1648C0;  /* Azul hover — ~10% mais escuro */
  --color-primary-light:    #EBF2FF;  /* Azul claro — fundos informativos, badges */
  --color-primary-dark:     #1240AD;  /* Azul escuro — estados pressionados */

  --color-accent:           #F97316;  /* Laranja energia — CTAs secundários, badges */
  --color-accent-hover:     #EA6C10;  /* Laranja hover */
  --color-accent-light:     #FFF4ED;  /* Laranja claro — fundos de destaque suave */
  --color-accent-dark:      #DC6309;  /* Laranja escuro — estado pressionado */

  /* ─── Cores Neutras ──────────────────────────────────────────── */
  --color-gray-950:         #0F172A;  /* Preto profundo — textos principais, header dark */
  --color-gray-800:         #1E293B;  /* Cinza muito escuro — fundos dark secundários */
  --color-gray-700:         #334155;  /* Cinza escuro — textos em fundo claro */
  --color-gray-500:         #64748B;  /* Cinza médio — textos secundários, legendas */
  --color-gray-300:         #CBD5E1;  /* Cinza claro — bordas, separadores */
  --color-gray-200:         #E2E8F0;  /* Cinza muito claro — fundos de inputs, hover sutil */
  --color-gray-100:         #F1F5F9;  /* Cinza ultra claro — fundos alternados */
  --color-gray-50:          #F8FAFC;  /* Off-white — fundo de seções alternadas */

  --color-white:            #FFFFFF;
  --color-black:            #000000;

  /* ─── Cores de Sistema ───────────────────────────────────────── */
  --color-success:          #10B981;  /* Verde — métricas positivas, confirmações */
  --color-success-light:    #ECFDF5;
  --color-warning:          #F59E0B;  /* Amarelo — atenção, avisos */
  --color-warning-light:    #FFFBEB;
  --color-error:            #EF4444;  /* Vermelho — erros, alertas críticos */
  --color-error-light:      #FEF2F2;
  --color-info:             #3B82F6;  /* Azul claro — informativos */
  --color-info-light:       #EFF6FF;

  /* ─── Gradientes ─────────────────────────────────────────────── */
  --gradient-primary:       linear-gradient(135deg, #1A56DB 0%, #3B82F6 100%);
  --gradient-accent:        linear-gradient(135deg, #F97316 0%, #FB923C 100%);
  --gradient-dark:          linear-gradient(135deg, #0F172A 0%, #1E293B 100%);
}
```

### 1.2 Tipografia

```css
:root {
  /* ─── Família ────────────────────────────────────────────────── */
  --font-family-base:       'Inter', -apple-system, BlinkMacSystemFont,
                            'Segoe UI', sans-serif;

  /* ─── Escala de tamanhos ─────────────────────────────────────── */
  --font-size-hero:         3.5rem;    /* 56px — título hero */
  --font-size-h1:           3rem;      /* 48px — H1 páginas internas */
  --font-size-h2:           2.25rem;   /* 36px — H2 seções */
  --font-size-h3:           1.75rem;   /* 28px — H3 cards/sub-seções */
  --font-size-h4:           1.375rem;  /* 22px — H4 items menores */
  --font-size-lead:         1.25rem;   /* 20px — parágrafo de introdução */
  --font-size-body:         1rem;      /* 16px — corpo padrão */
  --font-size-small:        0.875rem;  /* 14px — legendas, notas */
  --font-size-xs:           0.75rem;   /* 12px — badges, labels */

  /* ─── Pesos ──────────────────────────────────────────────────── */
  --font-weight-regular:    400;
  --font-weight-medium:     500;
  --font-weight-semibold:   600;
  --font-weight-bold:       700;
  --font-weight-extrabold:  800;

  /* ─── Line-heights ───────────────────────────────────────────── */
  --line-height-tight:      1.2;   /* Títulos grandes */
  --line-height-snug:       1.35;  /* Subtítulos */
  --line-height-normal:     1.5;   /* Padrão */
  --line-height-relaxed:    1.7;   /* Corpo de texto */
}
```

### 1.3 Espaçamento (base 8pt)

```css
:root {
  --space-1:    0.25rem;   /*  4px */
  --space-2:    0.5rem;    /*  8px */
  --space-3:    0.75rem;   /* 12px */
  --space-4:    1rem;      /* 16px */
  --space-5:    1.25rem;   /* 20px */
  --space-6:    1.5rem;    /* 24px */
  --space-8:    2rem;      /* 32px */
  --space-10:   2.5rem;    /* 40px */
  --space-12:   3rem;      /* 48px */
  --space-16:   4rem;      /* 64px */
  --space-20:   5rem;      /* 80px */
  --space-24:   6rem;      /* 96px */
  --space-32:   8rem;      /* 128px */

  --section-padding-y:      var(--space-20);  /* 80px vertical — desktop */
  --section-padding-y-sm:   var(--space-12);  /* 48px vertical — mobile */

  --container-max-width:    1200px;
  --container-padding-x:    var(--space-6);   /* 24px lateral */
}
```

### 1.4 Border Radius

```css
:root {
  --radius-sm:    4px;
  --radius-md:    8px;    /* inputs, cards menores */
  --radius-lg:    12px;   /* cards principais */
  --radius-xl:    16px;   /* containers maiores */
  --radius-2xl:   24px;   /* hero cards, elementos de destaque */
  --radius-full:  9999px; /* badges, pills */
}
```

### 1.5 Sombras

```css
:root {
  --shadow-sm:   0 1px 2px 0 rgba(15, 23, 42, 0.05);
  --shadow-md:   0 4px 6px -1px rgba(15, 23, 42, 0.07),
                 0 2px 4px -2px rgba(15, 23, 42, 0.05);
  --shadow-lg:   0 10px 15px -3px rgba(15, 23, 42, 0.08),
                 0 4px 6px -4px rgba(15, 23, 42, 0.05);
  --shadow-xl:   0 20px 25px -5px rgba(15, 23, 42, 0.10),
                 0 8px 10px -6px rgba(15, 23, 42, 0.05);
  --shadow-focus: 0 0 0 3px rgba(26, 86, 219, 0.35);
}
```

### 1.6 Z-index

```css
:root {
  --z-base:      0;
  --z-raised:    10;
  --z-dropdown:  20;
  --z-sticky:    30;
  --z-overlay:   40;
  --z-modal:     50;
  --z-toast:     60;
}
```

---

## 2. Componentes

### 2.1 Botões

#### Botão Primário

```css
.btn-primary {
  display:          inline-flex;
  align-items:      center;
  gap:              var(--space-2);
  padding:          var(--space-3) var(--space-6);
  background:       var(--color-primary);
  color:            var(--color-white);
  font-family:      var(--font-family-base);
  font-size:        var(--font-size-body);
  font-weight:      var(--font-weight-bold);
  line-height:      1;
  border:           none;
  border-radius:    var(--radius-md);
  cursor:           pointer;
  text-decoration:  none;
  transition:       background 0.2s ease, transform 0.1s ease, box-shadow 0.2s ease;
}

.btn-primary:hover {
  background:  var(--color-primary-hover);
  box-shadow:  var(--shadow-md);
  transform:   translateY(-1px);
}

.btn-primary:active {
  background:  var(--color-primary-dark);
  transform:   translateY(0);
}

.btn-primary:focus-visible {
  outline:     none;
  box-shadow:  var(--shadow-focus);
}

.btn-primary:disabled {
  background:  var(--color-gray-300);
  color:       var(--color-gray-500);
  cursor:      not-allowed;
  transform:   none;
}
```

#### Botão Secundário (outline)

```css
.btn-secondary {
  display:          inline-flex;
  align-items:      center;
  gap:              var(--space-2);
  padding:          calc(var(--space-3) - 2px) calc(var(--space-6) - 2px);
  background:       transparent;
  color:            var(--color-primary);
  font-family:      var(--font-family-base);
  font-size:        var(--font-size-body);
  font-weight:      var(--font-weight-bold);
  border:           2px solid var(--color-primary);
  border-radius:    var(--radius-md);
  cursor:           pointer;
  text-decoration:  none;
  transition:       background 0.2s ease, color 0.2s ease, transform 0.1s ease;
}

.btn-secondary:hover {
  background:  var(--color-primary-light);
  transform:   translateY(-1px);
}

.btn-secondary:focus-visible {
  outline:     none;
  box-shadow:  var(--shadow-focus);
}

.btn-secondary:disabled {
  color:        var(--color-gray-400);
  border-color: var(--color-gray-300);
  cursor:       not-allowed;
}
```

#### Tamanhos de botão

```css
.btn-sm { padding: var(--space-2) var(--space-4); font-size: var(--font-size-small); }
.btn-lg { padding: var(--space-4) var(--space-10); font-size: var(--font-size-lead); }
```

---

### 2.2 Cards

#### Card Padrão

```css
.card {
  background:     var(--color-white);
  border:         1px solid var(--color-gray-200);
  border-radius:  var(--radius-lg);
  padding:        var(--space-8);
  box-shadow:     var(--shadow-sm);
  transition:     box-shadow 0.25s ease, transform 0.25s ease, border-color 0.25s ease;
}

.card:hover {
  box-shadow:     var(--shadow-lg);
  transform:      translateY(-4px);
  border-color:   var(--color-primary);
}

.card-title {
  font-size:      var(--font-size-h3);
  font-weight:    var(--font-weight-bold);
  color:          var(--color-gray-950);
  margin-bottom:  var(--space-3);
}

.card-body {
  font-size:      var(--font-size-body);
  color:          var(--color-gray-500);
  line-height:    var(--line-height-relaxed);
}
```

#### Card de Métrica

```css
.card-metric {
  background:   var(--color-white);
  border:       1px solid var(--color-gray-200);
  border-radius: var(--radius-lg);
  padding:      var(--space-8);
  text-align:   center;
}

.card-metric-value {
  font-size:    var(--font-size-h1);
  font-weight:  var(--font-weight-extrabold);
  color:        var(--color-primary);
  line-height:  var(--line-height-tight);
  display:      block;
}

.card-metric-label {
  font-size:    var(--font-size-small);
  color:        var(--color-gray-500);
  margin-top:   var(--space-2);
  display:      block;
}
```

#### Card de Depoimento

```css
.card-testimonial {
  background:    var(--color-gray-50);
  border:        1px solid var(--color-gray-200);
  border-radius: var(--radius-lg);
  padding:       var(--space-8);
}

.card-testimonial-text {
  font-size:     var(--font-size-body);
  color:         var(--color-gray-700);
  line-height:   var(--line-height-relaxed);
  font-style:    italic;
  margin-bottom: var(--space-6);
}

.card-testimonial-author {
  display:     flex;
  align-items: center;
  gap:         var(--space-3);
}

.card-testimonial-avatar {
  width:        48px;
  height:       48px;
  border-radius: var(--radius-full);
  object-fit:   cover;
}

.card-testimonial-name {
  font-weight: var(--font-weight-semibold);
  color:       var(--color-gray-950);
}

.card-testimonial-role {
  font-size:   var(--font-size-small);
  color:       var(--color-gray-500);
}
```

---

### 2.3 Formulários

```css
.form-group {
  display:        flex;
  flex-direction: column;
  gap:            var(--space-2);
  margin-bottom:  var(--space-5);
}

.form-label {
  font-size:   var(--font-size-small);
  font-weight: var(--font-weight-semibold);
  color:       var(--color-gray-700);
}

.form-input,
.form-select,
.form-textarea {
  width:        100%;
  padding:      var(--space-3) var(--space-4);
  background:   var(--color-white);
  border:       1.5px solid var(--color-gray-300);
  border-radius: var(--radius-md);
  font-family:  var(--font-family-base);
  font-size:    var(--font-size-body);
  color:        var(--color-gray-950);
  transition:   border-color 0.2s ease, box-shadow 0.2s ease;
  outline:      none;
  appearance:   none;
}

.form-input::placeholder,
.form-textarea::placeholder {
  color: var(--color-gray-500);
}

.form-input:hover,
.form-select:hover,
.form-textarea:hover {
  border-color: var(--color-gray-400);
}

.form-input:focus,
.form-select:focus,
.form-textarea:focus {
  border-color: var(--color-primary);
  box-shadow:   var(--shadow-focus);
}

.form-input.error,
.form-select.error,
.form-textarea.error {
  border-color: var(--color-error);
  box-shadow:   0 0 0 3px rgba(239, 68, 68, 0.2);
}

.form-error-message {
  font-size:   var(--font-size-small);
  color:       var(--color-error);
  display:     flex;
  align-items: center;
  gap:         var(--space-1);
}

.form-textarea {
  min-height: 120px;
  resize:     vertical;
}
```

---

### 2.4 Badges e Tags

```css
.badge {
  display:        inline-flex;
  align-items:    center;
  padding:        var(--space-1) var(--space-3);
  border-radius:  var(--radius-full);
  font-size:      var(--font-size-xs);
  font-weight:    var(--font-weight-semibold);
  letter-spacing: 0.025em;
  text-transform: uppercase;
}

.badge-primary  { background: var(--color-primary-light); color: var(--color-primary); }
.badge-accent   { background: var(--color-accent-light);  color: var(--color-accent);  }
.badge-success  { background: var(--color-success-light); color: var(--color-success); }
.badge-warning  { background: var(--color-warning-light); color: var(--color-warning); }
.badge-error    { background: var(--color-error-light);   color: var(--color-error);   }
.badge-neutral  { background: var(--color-gray-100);      color: var(--color-gray-700);}
```

---

### 2.5 Seções e Layout

```css
.section         { padding: var(--section-padding-y) 0; }
.section-alt     { background: var(--color-gray-50); }
.section-dark    { background: var(--gradient-dark); color: var(--color-white); }
.section-primary { background: var(--gradient-primary); color: var(--color-white); }

.container {
  max-width: var(--container-max-width);
  margin:    0 auto;
  padding:   0 var(--container-padding-x);
}

.section-title {
  font-size:     var(--font-size-h2);
  font-weight:   var(--font-weight-bold);
  color:         var(--color-gray-950);
  margin-bottom: var(--space-3);
  line-height:   var(--line-height-snug);
}

.section-title.light { color: var(--color-white); }

.section-subtitle {
  font-size:   var(--font-size-lead);
  color:       var(--color-gray-500);
  max-width:   600px;
  line-height: var(--line-height-relaxed);
}

.section-subtitle.light { color: rgba(255, 255, 255, 0.8); }

/* Grid de cards */
.grid-cards {
  display:               grid;
  grid-template-columns: repeat(3, 1fr);
  gap:                   var(--space-6);
}

@media (max-width: 1024px) {
  .grid-cards { grid-template-columns: repeat(2, 1fr); }
}

@media (max-width: 640px) {
  .grid-cards  { grid-template-columns: 1fr; }
  .section     { padding: var(--section-padding-y-sm) 0; }
  .section-title { font-size: var(--font-size-h3); }
}
```

---

## 3. Estados dos Componentes

| Estado | Comportamento |
|---|---|
| **Default** | Estilo base conforme definido acima |
| **Hover** | `translateY(-1px a -4px)` + sombra aumentada + cor primária em bordas |
| **Active / Pressed** | `translateY(0)` + cor levemente mais escura |
| **Focus** | `outline: none` + `box-shadow: var(--shadow-focus)` (anel azul 3px) |
| **Disabled** | Cores de cinza; `cursor: not-allowed`; sem animação |
| **Loading** | Spinner inline; botão fica disabled durante a operação |
| **Error** | Borda vermelha + mensagem de erro abaixo |
| **Success** | Ícone de check verde + mensagem de confirmação |

---

## 4. Acessibilidade (WCAG AA mínimo)

### 4.1 Contraste de Cor

| Combinação | Ratio | Status |
|---|---|---|
| Texto `#0F172A` em branco | 19.1:1 | ✅ AAA |
| Texto `#64748B` em branco | 5.1:1 | ✅ AA |
| Branco em azul `#1A56DB` | 5.3:1 | ✅ AA |
| Branco em laranja `#F97316` | 3.1:1 | ✅ AA (texto grande) — ⚠️ borderline para texto pequeno |
| Branco em `#0F172A` | 19.1:1 | ✅ AAA |

> **Atenção:** O laranja deve ser usado principalmente para ícones, bordas e elementos decorativos — não como fundo de texto corrido pequeno.

### 4.2 Foco e Teclado

- Todo elemento interativo deve ter `focus-visible` visível
- Anel de foco: `box-shadow: 0 0 0 3px rgba(26, 86, 219, 0.35)` — nunca `outline: none` sem substituto
- Skip link "Ir para o conteúdo principal" visível ao navegar por teclado

### 4.3 Semântica HTML

```html
<!-- Estrutura semântica correta -->
<main id="main-content">
  <section aria-labelledby="services-heading">
    <h2 id="services-heading">O que fazemos</h2>
  </section>
</main>

<!-- Ícones decorativos -->
<svg aria-hidden="true" focusable="false">...</svg>

<!-- Screen reader only -->
<span class="sr-only">texto para leitores de tela</span>
```

### 4.4 Classe Screen Reader Only

```css
.sr-only {
  position:    absolute;
  width:       1px;
  height:      1px;
  padding:     0;
  margin:      -1px;
  overflow:    hidden;
  clip:        rect(0, 0, 0, 0);
  white-space: nowrap;
  border:      0;
}
```

---

## 5. Motion (Animações e Transições)

### 5.1 Durações e Easings

```css
:root {
  --duration-fast:    150ms;  /* Hover de estado */
  --duration-normal:  250ms;  /* Transições de componente */
  --duration-slow:    400ms;  /* Animações de entrada */
  --duration-slower:  600ms;  /* Transições de página */

  --ease-default:     cubic-bezier(0.4, 0, 0.2, 1);
  --ease-out:         cubic-bezier(0, 0, 0.2, 1);
  --ease-in:          cubic-bezier(0.4, 0, 1, 1);
  --ease-spring:      cubic-bezier(0.34, 1.56, 0.64, 1);
}
```

### 5.2 Animação de Entrada (Scroll)

```css
@keyframes fadeSlideUp {
  from { opacity: 0; transform: translateY(24px); }
  to   { opacity: 1; transform: translateY(0); }
}

.animate-on-scroll { opacity: 0; }

.animate-on-scroll.is-visible {
  animation: fadeSlideUp var(--duration-slow) var(--ease-out) forwards;
}

/* Stagger para grids */
.animate-on-scroll:nth-child(2) { animation-delay: 100ms; }
.animate-on-scroll:nth-child(3) { animation-delay: 200ms; }
.animate-on-scroll:nth-child(4) { animation-delay: 300ms; }
```

### 5.3 Preferência por Movimento Reduzido

```css
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration:        0.01ms !important;
    animation-iteration-count: 1 !important;
    transition-duration:       0.01ms !important;
    scroll-behavior:           auto !important;
  }
}
```

### 5.4 Regras Gerais

- ✅ Animações com propósito — indicar mudança de estado ou dar feedback
- ✅ Máximo 600ms para qualquer transição de UI
- ✅ Sempre implementar `prefers-reduced-motion`
- ❌ Sem loops automáticos sem controle do usuário
- ❌ Sem piscar elementos (risco de acessibilidade)
- ❌ Animar somente `transform` e `opacity` (não `width`, `height` — evita reflow)

---

*Fim do documento de Design Guidelines v1.0*
