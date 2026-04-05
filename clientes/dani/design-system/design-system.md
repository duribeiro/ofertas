# Design System — Dani Mentoria Tributária

> Baseado nas referências G4K (marketing digital)
> Criado: 2026-04-04

---

## 🎨 Paleta de Cores

### Cores Primárias

| Nome | Hex | Uso |
|------|-----|-----|
| **Azul Profundo** | `#0d1b2a` | Background principal, headlines |
| **Azul Médio** | `#1b263b` | Backgrounds secundários, cards |
| **Azul Claro** | `#415a77` | Elementos de suporte |

### Cores de Destaque

| Nome | Hex | Uso |
|------|-----|-----|
| **Amarelo Vibrante** | `#f9c74f` | CTAs, destaques, acentos |
| **Dourado** | `#ffd60a` | Highlights, ícones importantes |
| **Coral/Rosa** | `#e63946` | Alertas, urgência |
| **Verde Água** | `#2ec4b6` | Elementos de suporte, sucesso |

### Cores Neutras

| Nome | Hex | Uso |
|------|-----|-----|
| **Branco** | `#ffffff` | Texto sobre fundo escuro |
| **Cinza Claro** | `#e0e1dd` | Backgrounds alternativos |
| **Cinza Médio** | `#778da9` | Texto secundário |

### Gradientes

```css
/* Gradiente principal (hero, backgrounds) */
--gradient-primary: linear-gradient(135deg, #0d1b2a 0%, #1b263b 50%, #415a77 100%);

/* Gradiente de destaque (CTAs, destaques) */
--gradient-accent: linear-gradient(135deg, #f9c74f 0%, #ffd60a 100%);

/* Gradiente suave (cards, seções) */
--gradient-soft: linear-gradient(180deg, #0d1b2a 0%, #1b263b 100%);
```

---

## 🔤 Tipografia

### Fontes

**Headlines (títulos grandes):**
- Fonte: `Inter` ou `Poppins` (Google Fonts)
- Peso: 700 (Bold) ou 800 (Extra Bold)
- Tamanhos: 48px - 96px

**Subtítulos:**
- Fonte: `Inter` ou `Poppins`
- Peso: 500 (Medium) ou 600 (Semi Bold)
- Tamanhos: 24px - 36px

**Corpo de texto:**
- Fonte: `Inter` (fallback: Arial, sans-serif)
- Peso: 400 (Regular)
- Tamanho: 16px - 18px

**Texto secundário/captions:**
- Fonte: `Inter`
- Peso: 300 (Light) ou 400 (Regular)
- Tamanho: 12px - 14px

### Hierarquia Tipográfica

```css
/* Hero Title */
.hero-title {
  font-family: 'Inter', sans-serif;
  font-weight: 800;
  font-size: 72px;
  line-height: 1.1;
  color: #ffffff;
}

/* Section Title */
.section-title {
  font-family: 'Inter', sans-serif;
  font-weight: 700;
  font-size: 48px;
  line-height: 1.2;
  color: #ffffff;
}

/* Subtitle */
.subtitle {
  font-family: 'Inter', sans-serif;
  font-weight: 500;
  font-size: 24px;
  line-height: 1.4;
  color: #e0e1dd;
}

/* Body */
.body-text {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 16px;
  line-height: 1.6;
  color: #ffffff;
}

/* Caption */
.caption {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 14px;
  line-height: 1.5;
  color: #778da9;
}
```

---

## 📐 Layout e Espaçamento

### Grid

- Container máximo: `1440px`
- Padding horizontal: `48px` (mobile: `24px`)
- Gap entre elementos: `24px` - `48px`

### Espaçamento

| Nome | Valor | Uso |
|------|-------|-----|
| **xs** | `8px` | Micro espaçamentos |
| **sm** | `16px` | Padding interno de cards |
| **md** | `24px` | Gap entre elementos |
| **lg** | `48px` | Seções |
| **xl** | `72px` | Grandes seções |
| **2xl** | `96px` | Hero sections |

---

## 🔷 Elementos Visuais

### Formas Geométricas

**Círculos (decorativos):**
```css
.circle-accent {
  width: 200px;
  height: 200px;
  border-radius: 50%;
  background: linear-gradient(135deg, #f9c74f 0%, #ffd60a 100%);
  opacity: 0.2;
  position: absolute;
}
```

**Linhas diagonais:**
```css
.diagonal-line {
  height: 2px;
  background: linear-gradient(90deg, transparent 0%, #f9c74f 50%, transparent 100%);
  transform: rotate(-15deg);
}
```

### Cards

```css
.card {
  background: linear-gradient(180deg, #1b263b 0%, #0d1b2a 100%);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 16px;
  padding: 32px;
  box-shadow: 0 4px 24px rgba(0, 0, 0, 0.3);
}
```

### Botões

**Primário (CTA):**
```css
.btn-primary {
  background: linear-gradient(135deg, #f9c74f 0%, #ffd60a 100%);
  color: #0d1b2a;
  font-weight: 600;
  padding: 16px 32px;
  border-radius: 8px;
  border: none;
  cursor: pointer;
  transition: transform 0.2s, box-shadow 0.2s;
}

.btn-primary:hover {
  transform: translateY(-2px);
  box-shadow: 0 8px 24px rgba(249, 199, 79, 0.4);
}
```

**Secundário:**
```css
.btn-secondary {
  background: transparent;
  color: #ffffff;
  font-weight: 500;
  padding: 16px 32px;
  border-radius: 8px;
  border: 2px solid rgba(255, 255, 255, 0.3);
  cursor: pointer;
  transition: border-color 0.2s, background 0.2s;
}

.btn-secondary:hover {
  border-color: #f9c74f;
  background: rgba(249, 199, 79, 0.1);
}
```

---

## 🎭 Estilo Visual

### Identidade

- **Estilo:** Moderno, profissional, clean
- **Mood:** Confiança, expertise, sofisticação
- **Vibe:** Consultoria premium, tributário

### Elementos Recorrentes

1. **Gradientes suaves** em backgrounds
2. **Formas geométricas** como decoração
3. **Ícones minimalistas** (outline style)
4. **Tipografia forte** com hierarquia clara
5. **Contraste alto** (texto claro sobre fundo escuro)
6. **Espaçamento generoso**
7. **Bordas arredondadas** (8px - 16px)

### Ícones

- Estilo: Outline (linha)
- Espessura: 2px
- Tamanho: 24px - 48px
- Cor: Branco ou amarelo (destaques)

---

## 📄 Estrutura de Slides/Seções

### Hero Section
- Título grande (72px+)
- Subtítulo explicativo
- CTA principal (botão amarelo)
- Elemento visual decorativo (círculo, gradiente)

### Seção de Conteúdo
- Título de seção (48px)
- Cards com ícones
- Texto explicativo
- Call-to-action secundário

### Seção de Dados/Números
- Números grandes (destaque)
- Labels explicativos
- Gráficos simples (barras, círculos)

### Seção Final/CTA
- Mensagem de fechamento
- Botão de ação principal
- Contato/informações

---

## 🖼️ Aplicações

### Brand Book
- Capa com logo e nome
- Índice visual
- Seções de cores, tipografia, elementos
- Exemplos de aplicação

### Apresentação (PDF)
- Slides hero com título
- Slides de conteúdo
- Slides de fechamento
- Totalmente navegável

### Posts Redes Sociais
- Layout adaptado (1080x1080, 1080x1920)
- Elementos visuais consistentes
- Texto legível em mobile

---

## 📁 Arquivos Gerados

- `design-system.md` — Este arquivo
- `brand-book.html` — HTML do brand book
- `brand-book.css` — Estilos CSS
- `brand-book.pdf` — PDF final (via print)

---

_Design System criado para Dani Mentoria Tributária_
_Baseado nas referências G4K Marketing Digital_