---
status: Não iniciado # [Não iniciado | Em andamento | Concluído]
nome: ""
tipo_mecanica: "" # [Saber Ancestral | Interação com Cenário | Movimentação | Ilusão/Miragem]
local_desbloqueio: "[[Aldeia_Nome]]"
npc_mentor: "[[NPC_Nome]]"
item_requerido: "[[Item_Nome]]"
---

## ⚙️ Visão Geral & Game Design
- **Conceito:** [O que esse Saber faz na prática? Ex: Quebrar ilusões, revelar pegadas, apagar queimadas]
- **Utilidade no Mundo:** [Como o jogador usa fora do confronto?]
- **Aplicação contra Entidades/Espíritos:** [Qual desafio/espírito este saber resolve?]

---

## 🎮 Controles e Feedback Audiovisual
- **Comando / Input:** [Ex: Botão de ação, segurar botão para canalizar]
- **Feedback Visual (VFX):** [Partículas, alteração de shader de tela, brilho]
- **Feedback Sonoro (SFX):** [Som de instrumento, sopro do vento, águas]

---

## 💻 Lógica no Código (Variáveis Globais)
```javascript
// Exemplo da estrutura de estado global
const gameState = {
    aldeias_visitadas: ["cerrado", "pantano"], // Define avanço do tempo e ordem
    saberes_adquiridos: ["amuleto_protecao", "plantio"], // Desbloqueia mecânicas
};

// Exemplo de verificação de uso da mecânica
function ativarSaber(saberId) {
    if (gameState.saberes_adquiridos.includes(saberId)) {
        // Dispara efeito no mundo ou puzzle
        return true;
    }
    return false;
}
```

---

## 🧩 Puzzles e Barreiras Relacionadas
- [ ] Barreira no mapa bloqueada até obter este saber
- [ ] Puzzle em aldeia dependente deste aprendizado