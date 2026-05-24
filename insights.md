---
layout: page
title: "insights"
---

# ⚔️ RagnaHow

## Role Play Quests

- 12 relógios de spawn fixo

## 💡 Propostas

- Lista de quests revisada e NPCs específicos com lore
- Monstros Campeões
  - 🟥 Mob com 10x HP, 10x EXP, 10x DROP, 10x ATK, 10x MATK
  - 🟦 Mob igual com 10x EXP
  - 🟩 Mob igual com 10x spawn slaves agressivos
  - 🟨 Mob igual com 10x rolagens de drop

- ROTD novo a cada 2 hora, sendo leiloada a próxima raça com lance inicial de 100k. Default é raça aleatória caso ninguém dê lance.
- Hats rops fáceis de fazer podem facilitar a obtenção de caixas de hats (3 hats por 1 cx)
- MATQ no livro ou MATQ & ATQ em todas as armas (apenas Crusader usar ATQ&MATQ, sendo um benefício maior apenas para ele, mas simplifica este random option)
- Carta Creamy para fazer Asa Ilimitada
- Disponibilizar no menu da conta no site as contagens de kills do drop garantido
- Resetar mensalmente o ranking MVP e premiar com algum cosmético que expira em 1 mês.

- Monstros
  - Pasana
  - Anubis
  - IRON_FIST
  - SKELETON_GENERAL
  - WRAITH_DEAD
  - CAT_O_NINE_TAIL
  - Larva de Andre
  - Soldado de Andre
  - ELDER
- Drop
  - Gakkung[2] no Orc Archer
- Boss
  - Boss tipo planta
  - Boss com habilidades de veneno
  - Boss tipo Anjo
  - Boss elemento Sagrado
- Map
  -
- Manter da sala VIP
  - Utilidades
  - Mr Peso
  - Refino
  - Armas
  - Armaduras
  - Plágio
  - Arena PVP
  - Encantador Visuais EXP
  - Barricada (DPS Tester)
  - Estilista
  - Reciclagem
  - Curandeira
  - Venda Zeny
  - Doação
  - Máquina de Evento
  - Howssino
  - Conversor Visual
  - Slot Move
- Remover ao VIP
  - Habilidades de Platina
- Adicionar à sala VIP
  - Kafra com teleporte pago para todas as cidades

## 🐞 Bug

- **IA de Alvo:** Mobs que deveriam mudar de alvo facilmente não o fazem. Eles fixam no primeiro alvo que entra no raio de visão, mesmo que inalcançável, tornando-se alvos fáceis (afeta inclusive MVPs).
- Remover delay de teleport de 5s quando não há MVP
- prt_maze03

## ⚡ QoL

- Aumentar o tempo de permanência do loot no chão.
- Area loot de 1x1
- Remover limite de repetição de mensagens iguais 3 vezes
- Possibilitar @follow seguir o personagem de uma conta específica que esteja logado
- Habilitar botão direito do mouse para seguir
- Armas iniciais de iniciante com o

## 📜 Skills

### 🛡️ Swordsman

#### 🏇 Knight

#### 🛡️ Crusader

### 🧙 Mage

- **Energy Coat:** Não drenar SP em situações de dano 0 garantido (Pneuma, Safety Wall).
- **Firewall:** Mobs muito rápidos "furam" a parede. Sugestão: aumentar o delay do hit no mob.
  - default_walk_delay: 300 at conf\battle\skill.conf ffe40def4ab753b428f4425cdd946a56c7ae947a

#### 🧙‍♂️ Wizard

- Storm Gust
  - Em old times, o empurrão da nevasca é mais previsível, empurrando-os na direção nordeste quando não são atigindos pela borda sudoeste dela.

  conf/battle/skill.conf

  On official servers, Storm Gust consists of 81 units that all deal 3x3 splash damage "away from center".
  Due to south-western cells being processed first, this usually leads to a knockback to the northeast.
  Knockback at the edges will be away from SG. Knockback direction can also be influenced by Ganbantein and Land Protector.
  If you punch a hole into SG it will for example create a "suck in" effect.
  If you disable this setting, the knockback direction will be completely random (eAthena style).

  stormgust_knockback: no

#### 📖 Sage

- Land Protector
  - Em old times, todas as células do LP devem anular danos de terreno. Atualmente as bordas ficam desprotegidas.
    conf/battle/skill.conf

  On official servers, players standing on the border (outer cell) of the Land Protector can still be affected/hit by AoE skills (if the skill has a splash effect, such as Storm Gust). The Athena behavior ignores AoE affects/hits while players are standing on the border. Official: 0 Legacy Athena: 1

  land_protector_behavior: 1

### 🏹 Archer

#### 🦅 Hunter

#### 🎸 Bard

#### 💃 Dancer

### ⚖️ Merchant

#### ⚒️ Blacksmith

#### ⚗️ Alchemist

### 🗡️ Thief

- **Steal:** Não gastar SP em alvos que já foram roubados com sucesso.

#### 👤 Assassin

#### 🎭 Rogue

- Plágio
  - As skills estão mesmo sendo plagiadas? Tomei um sonic blow do grand peco e não copiou a skill (sobrevivi ao ataque inclusive)

### ⛪ Acolyte

- **Angelus:** Remover a animação nos alvos afetados.
- **Teleport** Remover menu para level 1
  - conf/battle/skill.conf skip_teleport_lv1_menu
- **Warp Portal** Disponibilizar /memo destes mapas
  - cmd_fild08
  - cmd_fild09
  - moc_fild03
  - moc_fild15
  - moc_fild16
  - yuno_fild03
  - pay_arche
  - pay_fild0

#### ✝️ Priest

- **Magnificat:** Remover a animação nos alvos afetados.
- **Gloria:** Remover a animação nos alvos afetados.
- **Kyrie Eleison:** Remover a animação nos alvos afetados.

#### 👊 Monk
