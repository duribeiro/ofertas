# Design System V2 — Arquitetura Visual (Agnóstica a Cor)

> Desenvolvido com a técnica "Roube como um Artista" a partir das referências aprovadas.
> Estrutura projetada para funcionar com qualquer paleta, focada em textura, hierarquia e composição (Light & Dark modes).
> Data: 2026-04-04

---

## 🏛️ Filosofia Visual
A fusão entre a **autoridade clássica** (tipografia serifada) e a **agilidade digital** (elementos UI modernos, pílulas, dark mode com luzes). O design não depende de cor para ser premium; ele depende de luz, textura e contraste tipográfico.

---

## 🔤 Tipografia (O Contraste)

O segredo aqui é o contraste entre o tradicional e o moderno.

### 1. Fonte Display (Títulos e Destaques)
- **Estilo:** Serifada (Elegante, clássica, remete a "advogado/autoridade")
- **Famílias sugeridas:** `Playfair Display`, `Lora`, `Merriweather`, ou `Instrument Serif`
- **Uso:** Apenas em Headlines (H1, H2) ou palavras de impacto.
- **Exemplo:** "A conta sumiu. E agora?"

### 2. Fonte Base (Corpo, UI e Pílulas)
- **Estilo:** Sans-Serif (Limpa, geométrica, legibilidade)
- **Famílias sugeridas:** `Inter`, `Plus Jakarta Sans`, ou `Montserrat`
- **Uso:** Textos longos, subtítulos, botões, tags/pílulas.
- **Hierarquia de pesos:** 400 (Regular) para texto, 600 (Semi-bold) para ênfase em UI.

---

## 🌓 Tratamento de Background e Texturas

A cor de fundo nunca deve ser "chapada". O aspecto profissional vem das camadas invisíveis.

### Modo Light (Claro)
- **Base:** Cores off-white ou cinza extremamente claro (nunca `#FFFFFF` puro).
- **Textura:** Ruído digital (Noise/Grain) com opacidade muito baixa (2% a 5%).
- **Padrão (Pattern):** Linhas sutis (Gridlines) ou padrões geométricos quase imperceptíveis ao fundo para dar profundidade.

### Modo Dark (Escuro)
- **Base:** Tons profundos (preto, azul-marinho profundo ou verde-escuro quase preto).
- **Luzes de Fundo (Atmospherics):** Gradientes radiais esfumaçados (Glows/Auroras) colocados estrategicamente atrás de elementos centrais para "acender" o design.
- **Textura:** Ruído digital (Noise/Grain) overlay (5% a 10%) para dar aspecto tátil e premium.

---

## 💊 Elementos de Interface e UI

A composição dos elementos visuais traz a estética moderna.

### 1. "Pílulas" (Tags / Badges)
- **Formato:** Totalmente arredondado (`border-radius: 999px`).
- **Estilos:**
  - *Preenchida:* Cor de fundo opaca com texto contrastante.
  - *Outline:* Fundo transparente, borda fina de 1px.
  - *Glass:* Fundo semi-transparente com desfoque (backdrop-filter: blur).
- **Uso:** Categoria do post (ex: "Direito Digital", "Dica Prática"), status, ou marcações no topo da arte.

### 2. Imagens e Ilustrações
- **Estilo:** Elementos sem fundo (recortados em PNG).
- **Interação:** As imagens (ex: celulares, pessoas) devem sobrepor os fundos texturizados e interagir com as luzes. O brilho do fundo deve ajudar a recortar a silhueta da imagem.

### 3. Notificações e Caixas (Mockups)
- **Composição:** Recriar elementos de UI reais (como notificações do Instagram, caixas de erro) flutuando no design.
- **Sombras:** Sombras muito difusas e extensas (`box-shadow: 0 20px 40px rgba(0,0,0,0.2)`), nunca sombras duras. Isso cria a sensação de "flutuar" sobre o background.

### 4. Rodapés (Footer Anchors)
- **Composição:** O rodapé deve ter um "peso" visual. Pode ser ancorado por uma barra sólida, ou por uma composição de elementos geométricos fortes que dão base à página/arte, equilibrando a leveza do topo.

---

## 🎨 Aplicação de Paleta (Como Injetar a Cor)

Sendo o sistema agnóstico, as cores funcionam via "Tokens". Se usarmos a combinação **Verde + Amarelo** que você aprovou na Imagem 1, o sistema se adapta assim:

- **Surface Dark (Fundo Dark):** Verde muito escuro, quase preto.
- **Surface Light (Fundo Light):** Off-white levemente esverdeado.
- **Brand Primary (Marca):** Verde bandeira ou verde floresta profundo.
- **Accent (Destaque):** Amarelo vibrante/Dourado.
- **Glows (Luzes no modo Dark):** Gradientes radiais em verde esmeralda ou amarelo esfumaçado no fundo.
- **Pílulas:** Borda ou fundo usando a cor *Accent* (Amarelo) para chamar atenção sobre fundos escuros.

---

## 📐 Regras de Composição ("Cheat Sheet")

1. **Camada 1:** Base (Cor sólida).
2. **Camada 2:** Pattern (Grid de linhas muito sutil).
3. **Camada 3:** Luzes radiais (Apenas no Dark Mode ou áreas de destaque no Light).
4. **Camada 4:** Ruído (Grain overlay para unificar tudo).
5. **Camada 5:** Elemento Recortado / Notificação com sombra flutuante.
6. **Camada 6:** Tipografia com forte contraste de tamanho (Fonte Serifada GIGANTE para título + Sans-Serif pequena e legível para apoio).
7. **Camada 7:** Pílulas e Rodapé ancorando o design.

---
_Gerado a partir das preferências extraídas: Dark com luzes/textura, Light com grid, fontes contrastantes, estilo UI notification e pílulas._