# Identidade Visual — Gio AI

Este arquivo é a fonte de verdade para cores, tipografia e tokens visuais do Gio. Qualquer interface — app, web, docs, e-mails — deve seguir estas definições.

> **Mudança aqui = mudança em todos os repos.**
> Ao alterar qualquer valor neste arquivo, atualize os arquivos correspondentes em `gio-app`, `gio-backend` (páginas HTML inline) e qualquer outro repo com interface visual. Registre a mudança no commit.

---

## Cores

| Token | Hex | Uso |
|-------|-----|-----|
| `gold` | `#C8922A` | Cor primária — CTAs, destaques, nome da marca |
| `goldLight` | `#E8B84B` | Hover e estados ativos de elementos dourados |
| `navy` | `#1A2540` | Fundo principal escuro, app bar, textos de contraste alto |
| `navyLight` | `#243050` | Variante do navy para cards e superfícies secundárias |
| `cream` | `#F7F3EC` | Fundo da tela principal, cards claros |
| `stone` | `#E2D9CC` | Bordas, divisores, separadores |
| `text` | `#2C2C2C` | Texto principal do corpo |
| `muted` | `#6B6B6B` | Texto secundário, placeholders, legendas |
| `white` | `#FFFFFF` | Texto sobre fundos escuros, ícones em botões |

### Combinações aprovadas

| Fundo | Texto/Ícone |
|-------|-------------|
| `navy` | `white`, `gold` |
| `cream` | `text`, `navy`, `gold` |
| `gold` | `white` |
| `white` | `text`, `navy` |

---

## Tipografia

### Fontes

| Fonte | Uso |
|-------|-----|
| **Playfair Display** | Títulos e cabeçalhos — transmite sofisticação e calor |
| **DM Sans** | Corpo de texto, botões, labels — legível e moderno |

### Escala de texto

| Nível | Fonte | Tamanho | Peso | Cor padrão |
|-------|-------|---------|------|------------|
| `displayLarge` | Playfair Display | 40px | 700 | `navy` |
| `displayMedium` | Playfair Display | 32px | 700 | `navy` |
| `headlineMedium` | Playfair Display | 26px | 700 | `navy` |
| `headlineSmall` | Playfair Display | 22px | 400 | `navy` |
| `bodyLarge` | DM Sans | 20px | 400 | `text`, line-height 1.6 |
| `bodyMedium` | DM Sans | 18px | 400 | `text`, line-height 1.5 |
| `bodySmall` | DM Sans | 14px | 400 | `muted` |
| `labelLarge` | DM Sans | 16px | 500 | `white` |
| `labelSmall` | DM Sans | 11px | 500 | `gold`, letter-spacing 1.2 |

> Fontes grandes (20px+ para corpo) são intencionais — o público principal tem 45+ anos.

---

## Tokens de interface

| Token | Valor | Uso |
|-------|-------|-----|
| Border radius padrão | `10px` | Inputs, botões, cards |
| Border radius grande | `24px` | Cards principais, modais |
| Altura mínima de botão | `58px` | Área de toque ampla para acessibilidade |
| Padding horizontal | `20px` | Inputs e containers |
| Padding vertical | `18px` | Inputs |
| Espessura de borda | `2px` | Inputs e divisores |

---

## Estados de input

| Estado | Cor da borda |
|--------|-------------|
| Padrão | `stone` (`#E2D9CC`) |
| Focado | `gold` (`#C8922A`) |
| Fundo | `cream` (`#F7F3EC`) |

---

## Mascote (Gio)

O mascote do Gio é um coelhinho dourado com olhos azuis expressivos. Aparece na página de status da API e em contextos de apresentação.

Paleta do mascote:
- Pelo: `#F0D060` (amarelo dourado claro)
- Barriga/orelhas internas: `#FAC8A0` (pêssego)
- Olhos (íris): `#4A7FA5` (azul aço)
- Nariz: `#E8A070`
- Boca: `#C05838`

O SVG fonte está em `gio-backend/cmd/api/main.go` (página HTML da rota `/`).

---

## Tom de voz

O Gio fala com:
- **Calor** — como um amigo próximo, nunca como um sistema
- **Paciência** — nunca apressado, sempre disposto a repetir
- **Clareza** — frases curtas, sem jargão
- **Respeito** — trata o usuário como adulto experiente, não como alguém que "não entende de tecnologia"

---

## Referência de implementação

| Plataforma | Arquivo |
|-----------|---------|
| Flutter | `gio-app/lib/core/theme/gio_theme.dart` |
| Backend (HTML inline) | `gio-backend/cmd/api/main.go` |
| Docs/e-mails | Usar as cores e fontes acima via CSS ou equivalente |
