# LibreTV — Player M3U Open Source (AGPLv3)

Player web/PWA gratuito, sem anúncios e sem rastreamento para listas **M3U** e **Xtream Codes**, com suporte a **Multi-tela (2 canais simultâneos)**, **Modo Kids com PIN** e armazenamento 100% local no navegador.

> **Aviso Legal (Zero Conteúdo):** O LibreTV é exclusivamente um reprodutor de mídia. O projeto **não** fornece, hospeda, vende ou distribui canais, filmes, séries ou listas. Cada usuário é integralmente responsável pelas listas e URLs que adiciona.

---

## Recursos do MVP

- **Player HLS nativo (`hls.js`)**: reprodução direta no navegador com suporte a listas `.m3u` / `.m3u8` via URL, arquivo local ou credenciais Xtream.
- **Multi-tela (Split Screen)**: assista a 2 canais lado a lado com alternância rápida de áudio.
- **Perfis e Controle Parental**: alterne entre o perfil **Principal** e o **Modo Kids** (bloqueio por PIN para sair e filtro automático de categorias adultas).
- **Privacidade por padrão**: sem cadastro, sem cookies de rastreio e sem envio das suas listas para servidores de terceiros (`localStorage` local).
- **PWA Instalável**: pode ser instalado no celular, desktop ou TV com navegador como aplicativo.
- **Proxy CORS opcional (Docker)**: incluído em `proxy/server.js` para quem deseja rodar em rede local ou VPS própria e abrir streams `http://` ou sem cabeçalhos CORS.

---

## Como publicar grátis no GitHub Pages / Cloudflare Pages

1. Faça um fork ou suba este repositório para o seu GitHub.
2. Ative o **GitHub Pages** em *Settings → Pages → Deploy from a branch (`main` / `/root`)*.
3. Seu player ficará no ar gratuitamente em `https://seu-usuario.github.io/libre-tv/`.

---

## Proxy CORS opcional (Docker)

Se precisar abrir streams `http://` ou servidores que bloqueiam requisições diretas do navegador:

```bash
docker compose up -d
```

O proxy ficará disponível na porta `8787` (`http://localhost:8787/proxy?url=...`).

---

## Apoie o Projeto (Doações)

Este software é mantido gratuitamente pela comunidade. Se o LibreTV é útil para você, considere apoiar:

- **Pix:** `33196137000112` CNPJ
---

## Licença (AGPLv3 & Dual-License Comercial)

Este projeto é distribuído sob a licença **GNU Affero General Public License v3.0 (AGPLv3)** — veja o arquivo [`LICENSE`](./LICENSE).

- **Uso livre e aberto:** você pode usar, estudar, modificar e hospedar livremente, desde que mantenha o código-fonte aberto sob AGPLv3 (inclusive em modificações oferecidas via rede/SaaS).
- **Uso Comercial / White-Label:** provedores de internet (ISPs), empresas de TV corporativa ou projetos que desejem distribuir versões proprietárias/fechadas com marca própria podem adquirir uma **licença comercial separada** entrando em contato com o mantenedor.
