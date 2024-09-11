# Aula 5 - Arquitetura Geral de Motores de Jogos e Exemplos de Motores

## :gear: O que é um Motor de Jogo?
Um motor de jogo é um conjunto de ferramentas e bibliotecas que facilita o desenvolvimento de jogos. Ele fornece as funcionalidades básicas para criar gráficos, física, som, entrada de usuário, e muito mais.

### III. Exemplos de Motores de Jogos
- Unity
  - Um dos motores de jogo mais populares.
  - Suporte a 2D e 3D, com uma vasta biblioteca de ativos.
  - Linguagens de script: C#.
- Unreal Engine
  - Conhecido por seus gráficos de alta qualidade.
  - Usado em jogos AAA e desenvolvimento de simulações.
  - Linguagens de script: C++ e Blueprints (sistema visual).
- Godot
  - Um motor open-source que é leve e flexível.
  - Suporta desenvolvimento 2D e 3D.
  - Linguagens de script: GDScript, C#, VisualScript.
- CryEngine
  - Focado em gráficos realistas e ambientes de mundo aberto.
  - Utilizado em jogos como "Far Cry" e "Crysis".
  - Linguagens de script: C++ e CryScript.
- GameMaker Studio
  - Ideal para desenvolvimento de jogos 2D.
  - Possui uma interface amigável e fácil de usar.
  - Linguagens de script: GameMaker Language (GML).

## 🧱 Importância da Arquitetura do Motor de Jogo
A arquitetura de um motor de jogo define como os diferentes componentes interagem, o que impacta a performance, flexibilidade e escalabilidade do jogo.

### I. Componentes Principais da Arquitetura de um Motor de Jogo
- Sistema de Renderização
  - Responsável por desenhar os gráficos na tela.
  - Pode usar APIs como OpenGL, DirectX, ou Vulkan.
  - Gerencia texturas, shaders e modelos 3D.
- Sistema de Física
  - Simula interações físicas entre objetos, como colisões e gravidade.
  - Pode incluir motores de física como Bullet ou PhysX.
- Gerenciamento de Recursos
  - Carrega, organiza e gerencia recursos do jogo, como modelos, texturas, sons e scripts.
  - Garante que os recursos sejam carregados de forma eficiente.
- Sistema de Entrada
  - Captura e processa entradas do usuário, como teclado, mouse, e controle.
  - Permite que os jogadores interajam com o jogo.
- Sistema de Som
  - Gerencia a reprodução de efeitos sonoros e música de fundo.
  - Pode usar bibliotecas como FMOD ou Wwise.
- Inteligência Artificial
  - Implementa comportamentos não-jogadores (NPCs).
  - Inclui algoritmos de pathfinding, tomada de decisão e comportamento emergente.
- Sistema de Script
  - Permite que desenvolvedores adicionem lógica de jogo sem recompilar o código.
  - Pode usar linguagens de script como Lua ou Python.
- Gerenciamento de Cenários
  - Controla as diferentes fases ou níveis do jogo.
  - Pode incluir carregamento e descarregamento de níveis.
### II. Arquitetura Geral
- Modelo de Entidade-Componente-Sistema (ECS)
  - Um padrão arquitetural que separa dados (componentes) e lógica (sistemas).
  - Facilita a composição de entidades de forma flexível.
- Fluxo de Execução
  - O motor geralmente segue um ciclo de atualização, que inclui:
    - Processamento de entrada
    - Atualização da lógica do jogo
    - Atualização do sistema de física
    - Renderização
    - Processamento de som
