# Closet Virtual

Guarda-roupa pessoal com o Claude. Funciona como uma página (Artifact) no claude.ai:
não precisa de servidor nem de chave de API, e os dados ficam guardados na própria página,
visíveis só para a dona.

App publicado: https://claude.ai/artifact/R4sEkrMeJu1x2P79sqEZvG

## O que faz

- **Armário**: suba fotos das peças (inclusive fotos de looks inteiros). O Claude identifica cada peça,
  recorta a foto e cria a ficha (nome, categoria, cores, tecido, estações, formalidade, estilo).
  Busca e filtros por categoria. Toque numa peça para corrigir ou excluir.
- **Prints do Google Fotos**: já usa o guarda-roupa do Google Fotos? Tire prints da tela de Itens rolando a lista
  e suba todos de uma vez. O Claude separa cada peça da grade, ignora botões e abas, recorta cada uma e pula as que já estão no armário
  (com a opção "Adicionar mesmo assim").
- **Estou numa loja**: foto de uma peça na loja → mostra o que você já tem de parecido e com o que combina.
- **Looks**: peça um look em texto ("jantar de sexta, friozinho") e receba combinações com as suas peças.
- **Catálogo de inspirações**: vá guardando prints de looks do Instagram, Pinterest ou de qualquer site. Quando quiser, abra uma inspiração
  e o Claude monta o look com as suas peças; o resultado fica salvo junto da foto. Filtros de "ainda não montadas" e "já montadas".
- **Álbuns**: peças organizadas em Parte de cima (com subgrupos Sem manga, Manga curta, Manga longa e Suéteres), Parte de baixo (Calças, Saias e Shorts) e Peça única (Vestidos, Macacões e Macaquinhos), Parte de baixo, Terceira peça, Peça única, Calçado, Acessório, Praia e Fitness, com "+" para adicionar direto na categoria, e álbuns próprios (Trabalho, Favoritas…).
- **Álbuns de looks**: organize os looks salvos em álbuns como Looks de festa ou Looks de inverno.
- **Dossiê**: biotipo, estilos e cartela de cores (Inverno Brilhante), com as cores que favorecem e as que evitar. O Claude usa o dossiê ao montar looks e malas e ao avaliar peças na loja.
- **Malas**: viagens com destino, datas, tipo e estação; roupas, looks por dia e checklist com progresso. O Claude pode montar ou completar a mala.

## Código

Tudo está em `app/closet.html` (HTML, CSS e JS sem dependências). Ele usa as capacidades do Artifact:
`db` (catálogo, looks, malas e inspirações), `assets` (fotos) e `sample` (Claude com visão).
Para atualizar o app, edite o arquivo e publique de novo no mesmo endereço.
