# Relatório de Publicação — Site-vitrine Adega Sintonia 035

Data: 2026-10-21

## URL do site no ar
**https://leohdie3-star.github.io/adega-sintonia-035-site/**

## Repositório
- https://github.com/leohdie3-star/adega-sintonia-035-site (PÚBLICO)
- Branch `main`, commit `79649f5` — "Site-vitrine Adega Sintonia 035"
- Conteúdo: `index.html` + `assets/` (16 imagens)
- O repositório privado do sistema de gestão não foi tocado.

## Passos executados
1. `adega-site.zip` extraído para `C:\PontePC\work\adega-site\`.
2. Antes de publicar, conferi o `index.html` atrás de segredos: não tem chave, token nem senha. Só aparecem os links públicos da loja (WhatsApp 35 98876-9652 e 35 99707-4351, Instagram @adegasintonia) e CDNs públicas (three.js, GSAP, Google Fonts).
3. Repositório criado com `gh repo create --public` e código enviado.
4. GitHub Pages ativado pela API (fonte: branch `main`, pasta `/`).

## Verificação
- Status do build do Pages: `built` (pronto em cerca de 1 minuto).
- `GET /` → HTTP 200, título: "Adega Sintonia 035 — Bebidas geladas em Baependi/MG | Peça pelo WhatsApp".
- Imagens testadas: `assets/hero.jpg`, `assets/logo.jpg` e `assets/prod-skol.webp` → HTTP 200, com o tipo de arquivo correto.

## Pendências
Nenhuma. O `gh` não pediu nenhuma confirmação.

---

## Atualização de preços (v2) — 2026-10-21

Regra do Leo: onde as versões antigas tinham preços diferentes, vale o MAIOR.

**URL final:** https://leohdie3-star.github.io/adega-sintonia-035-site/

### O que mudou
| Produto | Antes | Agora |
|---|---|---|
| Heineken Premium Lager (long neck 330 ml) | R$ 7,99 | **R$ 8,99** |
| Carvão Especial p/ Churrasco (saco 3 kg) | R$ 18,90 | **R$ 19,90** |

### Passos executados
1. `adega-site-v2.zip` extraído numa pasta separada (`C:\PontePC\work\adega-v2-extract\`).
2. Comparei com a versão publicada: o `index.html` muda só nessas 2 linhas de preço. As 16 imagens de `assets/` são idênticas.
3. Troquei o `index.html` no repositório, fiz o commit `433e805` ("Atualiza precos: Heineken 8,99 e Carvao 19,90") e o push para `main`.

### Confirmação de que está no ar
- Build do Pages para o commit `433e805`: `built` (cerca de 50 s).
- `GET /` (sem cache) → HTTP 200. O HTML no ar é idêntico, byte a byte, ao `index.html` da v2.
- Preços lidos no site publicado: `heineken price:8.99` e `carvao price:19.90`. ✅
