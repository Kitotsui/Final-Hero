Final Hero

Um jogo 2D desenvolvido em C utilizando a biblioteca Raylib
, onde o jogador controla um herói que enfrenta um demônio em uma arena. O projeto foi feito com foco em animações, movimentação fluida, colisões e organização modular de código.

🎮 Demonstração
<img src="https://img.itch.zone/aW1hZ2UvMTA3ODcxMC82MTg2Nzk2LmdpZg==/original/IzGwCg.gif" width="600" alt="Gameplay Preview">


🧩 Funcionalidades

✅ Movimento lateral do herói
✅ Sistema de animações (parado, correndo, atacando, tomando dano)
✅ IA simples do demônio (movimento automático e ataque)
✅ Colisão entre herói e inimigo
✅ Estrutura modular com arquivos separados (main.c, texturas.c, texturas.h)
✅ Gerenciamento de sprites via Raylib

⚙️ Tecnologias Utilizadas

C (ANSI C)

Raylib 5.0

MinGW (GCC) ou outro compilador C compatível

Windows / Linux

🗂️ Estrutura do Projeto
final_hero/
│
├── main.c                 # Lógica principal do jogo
├── texturas.c             # Funções de carregamento das texturas
├── texturas.h             # Declaração das texturas e funções
├── assets/
│   ├── heroi/
│   │   ├── parado/
│   │   ├── correr/
│   │   ├── ataque/
│   │   └── tomou_ataque/
│   └── demonio/
│       ├── idle/
│       ├── walk/
│       └── attack/
└── README.md

🧠 Como Rodar o Projeto
🔹 1. Instale a Raylib

Se estiver no Windows (com MinGW):

git clone https://github.com/raysan5/raylib.git
cd raylib/src
mingw32-make PLATFORM=PLATFORM_DESKTOP

🔹 2. Compile o jogo

Na pasta do projeto:

gcc main.c texturas.c -o final_hero -lraylib -lopengl32 -lgdi32 -lwinmm

🔹 3. Execute!
./final_hero

🧙 Personagens
Personagem	Descrição
🦸 Herói	Controlado pelo jogador, pode correr e atacar.
😈 Demônio	Move-se automaticamente e colide com o herói.
🧱 Lógica de Colisão

A colisão entre o herói e o demônio é calculada com base em suas posições X/Y e largura/altura dos sprites, impedindo que eles se atravessem quando se encostam.

🧑‍💻 Autores

Rogério Coutinho
Desenvolvedor do projeto e aluno de Análise e Desenvolvimento de Sistemas no Instituto Federal do Triângulo Mineiro.
