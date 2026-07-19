# BRIEF DE DESIGN — "Chronicle / Sovereign" (Brenno Meneghel)

> Cole este brief no agente. Ele define a linguagem visual pra QUALQUER peça: anúncio de
> marketplace (foto + copy + ficha), UI ou material de marca. Objetivo: refinamento editorial,
> "simples bem feito com extravagâncias pontuais".

## 1. DNA / Filosofia
Refinamento italiano + Bauhaus (grid e função) + clean nórdico + sobriedade inglesa.
Editorial, tipo capa de jornal financeiro premium. Muito respiro (espaço em branco/negativo).
Grid rigoroso. Paleta contida com **UM acento** por peça. Nada de poluição, nada de "template".
Extravagância só em pontos escolhidos (um número gigante, um detalhe de vidro/glow), nunca no todo.

## 2. Tipografia
- **Manchete/headline:** Playfair Display (serif) — grande, peso 700, tracking negativo (-0.02em).
- **Kicker/rótulo:** Libre Franklin — UPPERCASE, peso 700, letter-spacing 0.2em, tamanho pequeno.
- **Corpo/legenda:** Inter (system-ui fallback).
- **Números/dados/preço:** JetBrains Mono (mono) — peso 700, dá ar técnico/financeiro.
- Hierarquia clássica de jornal: KICKER pequeno em cima → Headline serif grande → subtítulo → corpo.

## 3. Paleta (dual — escolher 1 modo por peça)
**Escuro "Sovereign Black":** fundo quase-preto; texto #f4f4f5 / #b8b8c0 / #7c7c88 (dim);
positivo #34d399 (verde), negativo #f87171 (vermelho), atenção #fbbf24 (âmbar), destaque #38bdf8 (azul).
**Claro "Financial Times":** fundo off-white/creme; texto #1e1e2e / #3f3f5f / #71717a;
positivo #065f46, negativo #9f1239, atenção #92400e, acento índigo #6366f1.
Régua/hairline: cinza translúcido. **Regra: 1 acento colorido por peça**, o resto neutro.

## 4. Superfícies & tratamento de imagem (CRÍTICO p/ anúncios)
- **Glassmorphism:** cartões/faixas de vidro fosco translúcido (blur ~12px) sobre o fundo,
  borda hairline sutil, sombra suave. Nada de branco/cor chapada.
- **Ambilight / ambient glass:** fundo = a própria imagem borrada e ampliada, criando um "glow"
  que vaza pelas laterais. Dá profundidade e moldura.
- **NUNCA cortar a imagem do produto.** Usar `object-fit: contain` (produto inteiro, sempre)
  e preencher as laterais/sobras com o ambilight (imagem borrada) — jamais crop/zoom que corta.
- Cantos levemente arredondados (6–10px). Superfícies respiram, não encostam nas bordas.

## 5. Ícones
- **Somente lucide-react** (traço fino, monocromático, geométrico). **ZERO emojis** — nunca.
- Ícone acompanha texto, mesmo peso visual do texto, cor neutra ou o acento da peça.

## 6. Layout / composição
- Grid rígido, alinhamento à esquerda (editorial), colunas claras.
- **Régua dupla** estilo NYT sob o cabeçalho (linha grossa + linha fina).
- Muito respiro entre blocos. Densidade baixa. Um foco por peça.
- Número/preço pode ser o "grito" da peça: mono, grande, com leve glow do acento.

## 7. Aplicado a ANÚNCIO de marketplace (foto+copy+ficha)
- **Foto principal:** produto inteiro (contain) centralizado, fundo ambilight da própria foto.
- **Kicker** (categoria/benefício) uppercase Franklin em cima.
- **Título** curto em Playfair; **bullets** de ficha técnica em Inter com hairlines separando.
- **Preço** em JetBrains Mono, grande, com o acento. Selo/badge de vidro pra "novo/oferta".
- Paleta neutra + 1 acento da marca do produto. Sem emoji, sem setas berrantes, sem template ML genérico.

## 8. Do / Don't
✔ respiro, grid, 1 acento, serif editorial, mono nos números, vidro, imagem inteira + ambilight, lucide.
✘ imagem cortada, cor chapada, muitos acentos, emojis, poluição, template genérico, texto espremido.
