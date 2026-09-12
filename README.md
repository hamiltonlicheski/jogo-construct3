# Odisseia

Roguelike de ação em pixel art ambientado na mitologia grega, desenvolvido na engine Construct 3.

Jogável em: https://hamiltonlicheski.github.io/jogo-construct3-/

## Sobre o contexto do projeto

Projeto desenvolvido para a disciplina **Experiência Criativa: Explorando Computação e Inteligência Artificial**, com prazo de 1 mês para construção.

## Status do projeto

Em desenvolvimento. O esqueleto principal do jogo já está funcional de ponta a ponta (geração de mapa, movimento, combate, sala de chefe), mas os sprites finais, o hub e o tutorial ainda estão em produção.

## Sobre o jogo

Após ser morto por Posêidon, Odisseu é ressuscitado por Hades sob uma condição: matar o deus do mar. Entre as investidas, ele usa um barco como base (hub) e, a cada tentativa, atravessa ilhas geradas proceduralmente, cada uma com inimigos temáticos e um chefe próprio.

O protótipo atual se passa na Ilha dos Lestrigões.

### Referências

- **The Binding of Isaac** — estrutura de salas e câmera fixa.
- **Hades** — progressão por câmaras e hub entre partidas.
- **Cult of the Lamb** — identidade visual.
- **Stardew Valley** — o golpe de espada em arco.

## O que já está funcionando

- **Geração procedural**: a cada partida, um algoritmo de random walk sorteia 7 salas numa grade 5x5, sempre partindo do centro. O mapa muda completamente a cada execução, e o jogo materializa sozinho as salas, as paredes (onde não há vizinho) e as portas (onde há conexão).
- **Combate e movimento**: Odisseu se move em 8 direções (WASD e setas), dá um golpe em arco na direção que encara, tem dash com recarga, perde vida ao encostar em inimigos (com breve invulnerabilidade após o dano) e coleta moedas que os inimigos derrubam ao morrer.
- **Salas ao estilo Isaac**: a câmera é travada por sala, então cada ambiente preenche a tela exatamente, e a transição acontece ao cruzar uma porta. Ao entrar numa sala com inimigos, todas as portas trancam — inclusive a de trás, sem fuga — e só reabrem quando a sala é limpa.
- **Chefe**: o jogo calcula automaticamente qual das salas geradas é a mais distante da entrada e posiciona o Lestrigão lá, com mais vida e dano que os inimigos comuns.

## O que falta

- Tutorial na sala inicial.
- Hub do barco.
- Substituição dos placeholders geométricos pelos sprites finais (em produção pela equipe).
- "Telegraph" do chefe (aviso visual antes do ataque, como em Hades) — adiado de propósito até os sprites finais estarem prontos.

## Escopo e próximos passos

O escopo original previa cinco ilhas, mas a prioridade atual é entregar uma ilha completa e polida, junto com o hub. A arquitetura do projeto está sendo organizada em folhas de eventos reutilizáveis, de forma que adicionar uma segunda ilha exija pouco trabalho adicional caso o tempo permita.

## Tecnologias

- Construct 3 (engine de desenvolvimento de jogos)
- Exportação HTML5, hospedado via GitHub Pages

## Autor

Desenvolvido por Hamilton.
