# 🏡 Mon Homelab

Ce dépôt documente la conception, la configuration et l'évolution de mon homelab personnel, centré autour d’un routeur MikroTik et d’un réseau segmenté pour héberger mes propres services à domicile.
[Voir le homelab en ligne](https://www.canva.com/design/DAGnoILc0_c/__cwmvbNbSGJTWIP6RKAGw/edit?utm_content=DAGnoILc0_c&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton).

# 🔧 Objectifs

    Apprendre les bases du réseau avancé (VLAN, routage, NAT, firewall, DNS, DHCP…).

    Héberger localement des services (VPS, monitoring, containers, etc.).

    Expérimenter la virtualisation, la sécurité réseau, et l’automatisation.

    Contourner les limitations imposées par ma box 5G (CG-NAT) grâce à un tunnel IP.

# 🧱 Infrastructure

    Routeur principal : MikroTik RB3011UiAS-RM

    Accès Internet : Box 5G (Routeur Arcadyan de chez Bouygues )

    Topologie réseau :

        LAN utilisateurs : 192.168.1.0/24

        LAN serveur : 192.168.88.0/24 (isolé derrière le MikroTik)

    Firewall : accès restreint à l’administration du routeur

    Tunnel IP : vers VeryCloud pour accéder aux services depuis l’extérieur (ainsi qu'avoir une protection Anti-DDOS)

    DHCP : contrôlé par le MikroTik sur les ports physiques du réseau serveur

# 🔒 Sécurité

    Accès au routeur restreint à une seule IP locale

    DHCP désactivé sur WAN

    NAT configuré uniquement côté WAN (masquerade)

    Isolation inter-VLAN (en cours)

# 📁 Contenu du dépôt

    🔹 /configs : fichiers de configuration MikroTik exportés

    🔹 /docs : schémas réseau, notes d’installation et de déploiement

    🔹 /scripts : scripts utiles pour backups, mises à jour ou maintenance
