---
status: Não iniciado # [Não iniciado | Em andamento | Concluído]
nome: ""
bioma: "" # [[Bioma_Nome]]
ameaca_principal: "" # [[Inimigo_Nome]]
saber_desbloqueado: "" # [[Mecanica_Nome]]
ordem_visita_impacto: true
---

## 📍 Resumo & Atmosfera
- **Conceito Visual:** [Descrição da aldeia, arquitetura tradicional, bioma ao redor]
- **Crise Atual:** [Qual desequilíbrio ou entidade está afetando a comunidade local?]

---

## ⏳ Requisitos de Entrada e Passagem do Tempo
O estado desta aldeia muda conforme a ordem em que o jogador decide visitá-la:

- **Se for a 1ª Aldeia visitada:** [Estado preservado, crise ainda em estágio inicial, NPCs ativos]
- **Se for a 2ª Aldeia visitada:** [Crise agravada, moradores acuados, parte do cenário corrompido]
- **Se for a 3ª Aldeia visitada:** [Colapso iminente, necessidade urgente de saberes de outras aldeias para resolver]

> [!NOTE] Saberes Recomendados
> Saberes que facilitam a exploração ou resolução de puzzles nesta aldeia:
> - [[Mecanica_SaberExemplo]]

---

## 🗣️ População & NPCs
| NPC | Papel / Ocupação | Saber / Item Entregue | Arquivo de Diálogo |
| :--- | :--- | :--- | :--- |
| **[[NPC_Lider]]** | Liderança da aldeia | Explica a crise | [[Dialogo_Lider]] |
| **[[NPC_Mentor]]** | Mestre do Saber | [[Saber_Nome]] | [[Dialogo_Mentor]] |

---

## 🧩 Puzzles e Conflito Local
- **Objetivo da Missão:** [O que o jogador precisa fazer para restaurar o equilíbrio?]
- **Solução Harmônica:** [Como resolver respeitando a natureza e a cultura local]

---

## 🎨 Assets Necessários
- [ ] Cenário base (Tilemap e prop tiles do bioma)
- [ ] Sprites de NPCs e animais locais
- [ ] Músicas e sons ambientes (fogueira, pássaros, chuva)