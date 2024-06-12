Decidimos fazer o jogo com a seguinte premissa: ele é
um complemento para ajudar uma pessoa a mestrar uma mesa
de RPG, dentro dele é possível simular exploração, combate
e progressão, e também armazenar o inventário dos eventuais
jogadores, deve ser utilizado pelo mestre da sessão como
um guia para ajudar nas funções básicas do jogo!

Localidades presentes para uso:
Aldeia
Floresta
Montanha
Caverna

Estrutura implementadas:

Listas: Utilizadas para armazenar habilidades (std::list<Habilidade>) 
dos personagens e monstros.

Vetores: Utilizados para armazenar inventário (std::vector<Item>) dos 
personagens e coleções de NPCs, itens e monstros em localidades 
(std::vector<NPC>, std::vector<Item>, std::vector<Monstro>).

Mapas: Utilizados para organizar a árvore de habilidades 
(std::map<std::string, NodoHabilidade*>) e para armazenar 
localidades e suas adjacências (std::unordered_map<std::string, Localidade> 
e std::unordered_map<std::string, std::vector<std::string>>).

Tabelas Hash: Utilizadas para acesso rápido a personagens e monstros 
(std::unordered_map<std::string, Personagem>, std::unordered_map<std::string, Monstro>).
