
<img src="https://github.com/LeoRuer/homelab/blob/main/docs/img/bgp.png?raw=true" alt="BGP" style="width:400px;"/>

"_En BTS SIO, tout ce qu'il y a après routage inter-vlan est hors programme._" Voici ce que m'a dit un jour mon formateur en informatique quand j'étais encore à l'armée. 
Quand on regarde le programme, c'est vrai que le niveau en termes de réseau ne vole pas très haut.
Ce dossier a pour but de regrouper mon parcours de montée en compétences et des labs pratiques autour de l’univers opérateur.

## ⚠️ Nota Bene

Je n'ai JAMAIS travaillé dans le domaine de l'hébergement ou encore des opérateurs. Je peux me tromper, être maladroit dans mes explications ou simplement oublier de parler de certains sujets. Je ne suis pas payé à rédiger ce que vous lisez. Je suis là pour apprendre, vous faire apprendre et c'est déjà pas mal non ?

---

## 🎯 Objectif

Ce dépôt a été conçu pour explorer **le cœur technique de l’Internet** :  
comment les FAI échangent du trafic, routent des préfixes IP, automatisent leur infrastructure, et assurent la haute disponibilité à l’échelle globale.

---

## 🧠 Ce que vous allez apprendre ici

### 📡 Routage opérateur (BGP, MPLS, OSPF)
- Création d’un réseau multi-AS avec **BGP**
- Utilisation des **AS-PATH, communities, local-pref** pour influencer les routes
- Mise en place de **MPLS** et de **VPN inter-sites**
- Redondance via **OSPF / redistribution / failover**

### 🛠 Provisioning & infrastructure physique
- Boot PXE / DHCP / kickstart pour installer automatiquement des serveurs
- Gestion de **l’infrastructure bare-metal** (IPMI, câblage, dual power)
- Mise en place de **ZTP-like** pour les équipements réseau

### 📊 Supervision & observabilité
- Collecte de métriques réseau avec **Zabbix / SNMP**
- Mise en place de dashboards et d’alertes
- Centralisation des logs avec **ELK** ou **Graylog**

### 🔐 Sécurité et bonnes pratiques FAI
- Mise en place de **RPKI / max-prefix / route filtering**
- Simulation d’attaques BGP (hijack, leak) et stratégies de mitigation
- Mise en œuvre du **RTBH (Remote Triggered Black Hole)**
