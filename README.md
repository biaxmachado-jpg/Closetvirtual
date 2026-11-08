# Closet Virtual

Guarda-roupa pessoal com o Claude. Funciona como uma página (Artifact) no claude.ai:
não precisa de servidor nem de chave de API, e os dados ficam guardados na própria página,
visíveis só para a dona.

App publicado: https://claude.ai/artifact/R4sEkrMeJu1x2P79sqEZvG

## O que faz

- **Armário**: suba fotos das peças (inclusive fotos de looks inteiros). O Claude identifica cada peça,
  recorta a foto e cria a ficha (nome, categoria, cores, tecido, estações, formalidade, estilo).
  Busca e filtros por categoria. Toque numa peça para corrigir ou excluir.
- **Estou numa loja**: foto de uma peça na loja → mostra o que você já tem de parecido e com o que combina.
- **Looks**: peça um look em texto ("jantar de sexta, friozinho") e receba combinações com as suas peças.
- **Inspiração**: suba um print do Instagram/Pinterest → equivalentes no seu armário, looks e o que falta.
- **Álbuns**: peças organizadas em Parte de cima, Parte de baixo, Terceira peça, Peça única, Calçado, Acessório, Praia e Fitness, com "+" para adicionar direto na categoria, e álbuns próprios (Trabalho, Favoritas…).
- **Malas**: viagens com destino, datas, tipo e estação; roupas, looks por dia e checklist com progresso. O Claude pode montar ou completar a mala.

## Código

Tudo está em `app/closet.html` (HTML, CSS e JS sem dependências). Ele usa as capacidades do Artifact:
`db` (catálogo, looks e malas), `assets` (fotos) e `sample` (Claude com visão).
Para atualizar o app, edite o arquivo e publique de novo no mesmo endereço.
