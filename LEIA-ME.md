# Site Apta Assessoria e Treinamentos

## Páginas
- index.html ................ Home (hero, cursos, metodologia, instrutoras, investimento, FAQ)
- curso-cuidador.html ....... Página do Curso de Cuidador (5 módulos, datas, material, certificado)
- inscricao.html ............ Formulário de inscrição
- trabalhe-conosco.html ..... Vagas e candidatura

A seção **Metodologia** fica dentro da home, em `index.html#metodologia`.

## Estrutura
```
index.html
curso-cuidador.html
inscricao.html
trabalhe-conosco.html
AptaLogo.dc.html      -> componente da logo (carregado pelas páginas)
support.js            -> runtime que renderiza as páginas
assets/               -> logo, capas e fotos dos cursos
uploads/              -> fotos das instrutoras e fontes da marca
```

## Como rodar localmente
As páginas usam `fetch` para carregar a logo, então precisam de um servidor HTTP (abrir o arquivo direto com file:// não funciona):

```bash
npx serve .
# ou
python3 -m http.server 8000
```

## Publicar no domínio
Suba a pasta inteira na raiz do servidor (public_html, /var/www/html, Netlify, Vercel, etc.). Nenhuma build é necessária — é HTML estático.

## Pendências para configurar
1. **Formulários** — `inscricao.html` e `trabalhe-conosco.html` hoje só mostram a tela de confirmação no navegador; não enviam dados. Conectar a um backend, Formspree, Google Forms ou webhook do WhatsApp.
2. **Fontes** — Equitan Sans e TT Lakes Neue são versões **Trial**. Adquirir a licença comercial antes de publicar.
3. **SEO** — incluir meta description, Open Graph, favicon e sitemap.
4. **Analytics** — instalar Google Analytics / Meta Pixel se for anunciar.
5. **Links externos** — WhatsApp (88) 8182-8291 e @aptacariri já estão configurados.

## Dados do curso usados no site
- 80 horas · 8 encontros presenciais · 7h–11h e 13h–17h
- Datas: 10 e 11/10 · 17 e 18/10 · 31/10 e 01/11 · 07 e 08/11 de 2026
- Local: Juazeiro do Norte – CE
- Investimento: R$ 400 (10% OFF no PIX = R$ 360) ou 12x de R$ 33,30
- Certificado de 80h · CBO 5162-10
