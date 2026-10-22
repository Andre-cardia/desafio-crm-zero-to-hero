# Abrir a apresentação interativa

A apresentação está em apresentacao.html e incorpora as imagens. Para carregar a animação Three.js, mantenha conexão com a internet e abra a página por um servidor local:

~~~bash
cd desafio-crm-zero-to-hero
python3 -m http.server 8000
~~~

Depois, acesse http://localhost:8000/apresentacao.html no navegador.

## Controles

- Seta para a direita ou esquerda: avançar e voltar.
- Home ou End: primeira e última tela.
- M: abrir o índice.
- N: mostrar notas do apresentador.
- F: tela cheia.
- Esc: fechar notas ou janelas.
- Também é possível usar os botões ou deslizar em telas de toque.

As imagens da abertura, do pré-projeto e da construção foram geradas para este material e estão embutidas no HTML. A cena Three.js usa partículas e relações entre nós para representar contatos e oportunidades; se o navegador bloquear a conexão com o CDN, os slides e controles continuam disponíveis.
