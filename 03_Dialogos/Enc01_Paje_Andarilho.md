---
status: Em andamento
personagem: "[[Paje_Andarilho]]"
local: Ponto de Descanso Inicial / Bifurcação das Águas
gatilho_aparecimento: Após o jogador finalizar a escolha inicial de gênero e sair do tutorial.
---

## 📍 Contexto da Cena
Este é o primeiro contato do jogador com o Pajé. O objetivo desta conversa é apresentar a mecânica de miragens e entregar o primeiro item de proteção (o amuleto trançado).

## 💬 Roteiro do Diálogo

**[Pajé Andarilho]**  
> *"Ah... as águas me avisaram que um novo caminhante despertaria hoje. A floresta está inquieta, jovem. O equilíbrio foi quebrado, e os antigos espíritos caminham com raiva."*

**[Opções de Resposta do Jogador]**
- **Opção A:** *"Quem é você?"*
  - **[Pajé Andarilho]:** *"Apenas um velho que escuta o vento. Mas o que importa agora não sou eu, e sim o caminho que está à sua frente."*
- **Opção B:** *"O que está acontecendo com a floresta?"*
  - **[Pajé Andarilho]:** *"A natureza reflete as feridas causadas pelos homens. E agora, essas feridas estão ganhando forma."*

---

### 🌿 Bloco Condicional (Ameaça Inicial)
Aqui, o diálogo se divide com base na variável `genero_player` definida no *Autoload*[cite: 1].

- **SE o jogador for Masculino (Rota da Iara):**  
  > **[Pajé Andarilho]:** *"Tenha cuidado ao se aproximar dos rios. A Iara canta alto hoje, tentando atrair os corações puros para o fundo das águas."*[cite: 1]
  
- **SE o jogador for Feminino (Rota do Boto):**  
  > **[Pajé Andarilho]:** *"Tenha cuidado ao visitar as festas da próxima aldeia. O Boto caminha disfarçado entre as sombras, espalhando ilusões para enganar os desavisados."*[cite: 1]

---

### 🎁 Finalização e Entrega de Item
**[Pajé Andarilho]**  
> *"Eles usam ilusões para confundir a mente. Leve isso com você. Os anciões me ensinaram a trançar este amuleto... ele vai te ajudar a ver o que é real quando a tela da sua mente se distorcer."*[cite: 1]

## 💻 Eventos para a Engine
Quando o diálogo acabar, rodar os seguintes comandos no código:
- [ ] Adicionar `"amuleto_protecao"` ao array `gameState.saberes_adquiridos`[cite: 1].
- [ ] Liberar a passagem (abrir o colisor) para a primeira aldeia.
- [ ] Ocultar o NPC da cena (ele só volta a aparecer no Encontro 2).