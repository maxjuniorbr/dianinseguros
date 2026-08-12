# Dianin Seguros

Site institucional de página única da Dianin Seguros - corretora de seguros em Mandaguari, PR.

## Site

**[https://dseg.com.br](https://dseg.com.br)**

## Sobre

Landing page do corretor Paulo César Dianin. HTML, CSS e JavaScript puros - sem frameworks, sem dependências e sem build. Tudo é servido estaticamente pelo GitHub Pages.

O objetivo da página é um só: levar o visitante ao WhatsApp do corretor com o assunto já preenchido.

## Estrutura

```
index.html                  # Página inteira (HTML + CSS + JS embutidos)
assets/
  fonts/                    # Archivo e Space Grotesk (subset latin, woff2)
  img/                      # Logo, retrato, favicons e imagem de compartilhamento
  img/seguradoras/          # Logos das seguradoras (silhuetas PNG monocromáticas)
```

## Desenvolvimento

Abra `index.html` no navegador. Não há etapa de build.

Para testar servindo os arquivos como em produção:

```bash
python3 -m http.server 8000
```

## Notas de implementação

- **Fontes**: Archivo (texto) e Space Grotesk (títulos), variáveis, subset latin, servidas do próprio domínio - nenhuma requisição externa.
- **Logos das seguradoras**: PNGs de silhueta branca exibidos como `<img>` com opacidade reduzida, que sobe no hover. Cada `<img>` carrega sua própria largura, ajustada logo a logo para equilíbrio óptico.
- **Sem JavaScript**: a página continua legível e navegável. O JS só adiciona a revelação no scroll, o botão flutuante do WhatsApp e o acordeão de uma dúvida aberta por vez.
- **SEO**: meta description, Open Graph, `InsuranceAgency` e `FAQPage` em JSON-LD.
