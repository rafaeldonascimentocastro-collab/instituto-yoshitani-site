# Instituto Yoshitani – Solidariedade e Cidadania

Site institucional do Instituto Yoshitani: voluntariado, doação de alimentos e apoio a idosos e crianças na Grande São Paulo.

Site estático (HTML/CSS/JS, sem dependências), publicado pelo GitHub Pages a cada push na branch `main`.

## Como atualizar dados

No final do `index.html`, edite o objeto `CONFIG`. Campos vazios ficam ocultos no site.

| Campo | O que ativa |
|---|---|
| `nomeOficial`, `cnpj`, `natureza`, `fundacao`, `missao` | Ficha em "Quem somos"; CNPJ também perto dos botões, no rodapé e na política de privacidade |
| `regiao` | Região usada nos textos do site |
| `email`, `agendaUrl` | Botões de e-mail e agenda para empresas; canal de e-mail no contato |
| `pixChave` | Bloco de doação via PIX |
| `instagramPosts` | Posts recentes do Instagram exibidos no site |
| `numeros`, `documentos` | Resultados documentados e documentos de transparência |
| `fotos` (`g1`…`g6`) | Galeria "Momentos" (só aparece com fotos autorizadas) |
| `formEndpoint` | Cópia das inscrições em planilha (Google Apps Script ou Formspree) |
| `ga4Id` ou `plausibleDomain` | Medição de visitas e cliques nos botões |

## Domínio próprio

Ao publicar em domínio próprio, troque a URL atual em `index.html` (canonical, og:url, og:image, JSON-LD e `CONFIG.siteUrl`), `robots.txt` e `sitemap.xml`, e crie o arquivo `CNAME` com o domínio.

## Arquivos

- `index.html` — site completo.
- `assets/` — logotipos, ícones, imagem de compartilhamento (`og-image.jpg`) e fotos otimizadas em WebP.
- `robots.txt`, `sitemap.xml`, `site.webmanifest` — indexação e ícones.
