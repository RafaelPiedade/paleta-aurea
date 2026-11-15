# Paleta Áurea

Ferramenta de estudo de cor para web e redes sociais: gera paletas pela proporção áurea, sugere o destaque de uma dupla de cores, monta cores no espaço HSL em 3D e mostra o que cada cor transmite.

**🔗 Demo: [rafaelpiedade.github.io/paleta-aurea](https://rafaelpiedade.github.io/paleta-aurea/)**

## Modos

### Proporção áurea
Parte de **uma cor** e gera uma paleta de três:
- **Acento:** gira o ângulo áureo (360° − 360°/1,618 ≈ **137,5°**) no círculo cromático, em RYB (círculo dos pintores) ou RGB (telas).
- **Suporte:** a mesma matiz com menos saturação e mais luz.
- Distribuição 60 · 30 · 10 e escala tipográfica áurea (13 → 21 → 34 → 55 px).

### Dupla + destaque
Parte de **duas cores** (uma viva e um fundo neutro) e sugere a terceira por dois caminhos:
- **Contraste:** 105–165° no círculo RYB, temperatura oposta.
- **Mesma família:** ±7,5°, tom sobre tom.
- Grade de candidatos em quatro variações (mesmo brilho, vivo, pastel, neon) e combinações prontas.

### Montar cor
- Cole uma cor em **HEX, RGB, HSL, HSB** ou nome CSS.
- Ajuste por HSL, HSB ou RGB com barras que mostram o resultado.
- **Círculo cromático** clicável (matiz e saturação).
- **Espaço HSL em 3D** (cilindro ou cone duplo): arraste para girar e clique para escolher.
- Valores em HEX, RGB, HSL, HSB e OKLCH, contraste WCAG, harmonias e escala de tons 50–900.

### Psicologia das cores
- Análise de qualquer cor: família, tom (pastel, vibrante, escuro, terroso…), o que transmite, cuidados e onde usar.
- Busca por intenção (confiança, luxo, calma, urgência…).
- Ficha rápida de 13 cores, com as campanhas de conscientização do calendário brasileiro (Outubro Rosa, Novembro Azul…).

### Em todos os modos
- Clique em qualquer cor para copiar.
- Exportação em HEX, CSS, SCSS, Tailwind, JSON e texto.
- Prévia de tipografia com Google Fonts e de composição.
- Paletas salvas no navegador, tema claro e escuro, e estado guardado na URL para compartilhar.

## Atalhos

| Tecla | Ação |
|---|---|
| `1` `2` `3` | Copiam cada cor |
| `A` | Copia a paleta |
| `R` | Cor aleatória |
| `M` | Troca o modo |
| `T` | Troca o tema |
| `⌘V` / `Ctrl+V` | Cola uma cor no modo Montar cor |

## Rodar localmente

É um único arquivo HTML, sem dependências nem build. Abra o `index.html` no navegador ou sirva a pasta:

```bash
python3 -m http.server 8000
```

Depois acesse `http://localhost:8000`.

## Tecnologias

HTML, CSS e JavaScript puros, com Canvas 2D para o círculo e o espaço 3D. As fontes vêm do Google Fonts.
