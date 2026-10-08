NetMap Architect est un outil de cartographie topologique et logique de réseaux, pensé pour les architectes système, les ingénieurs réseau et les auditeurs cybersécurité.

Conçu à contre-courant des solutions lourdes du marché (Visio, Packet Tracer), NetMap a été forgé autour d’une philosophie stricte : Zéro latence, Zéro dépendance, Zéro télémétrie. C’est un Single-File Application (Application en un seul fichier) qui s’exécute intégralement côté client. Il comprend le vocabulaire réseau (VLANs, sous-réseaux, tables de routage) et génère des schémas interactifs d’une précision chirurgicale.

-  Caractéristiques Principales (The Laser Features)

- Air-Gapped & Privacy First (Zéro Cloud)
100% Client-Side : L’outil est un unique fichier .html. Aucun serveur back-end, aucun tracking, aucune API externe.
Bunker Ready : Peut s’exécuter sur une machine isolée sans aucune connexion internet. Idéal pour cartographier des environnements restreints (OT/SCADA, Défense, Datacenters sensibles).

- Moteur d’Analyse VLAN Intelligent (Smart Parsing)
Syntaxe Naturelle : Saisissez simplement "10, 20, 100-105, TRUNK" dans un lien. Le moteur Regex interprète les plages, génère dynamiquement la palette de couleurs, et crée les badges associés.
Highlight Mapping : Un clic sur un VLAN dans la légende (ou sur un badge) met en surbrillance l’intégralité du parcours de ce VLAN (câbles et équipements) sur la topologie, tout en assombrissant le reste. Parfait pour le troubleshooting (Spanning-Tree, flux routés).

- Géométrie et UX “Pixel-Perfect”
Algorithme de Câblage Dynamique : Les liens sont calculés mathématiquement pour cibler les centres de gravité des équipements avec un offset dynamique, empêchant le chevauchement des câbles.
Routage Visuel Personnalisé : Chaque faisceau de câbles possède un point de bascule modifiable (Drag & Drop) permettant de contourner les éléments visuels et d’organiser proprement les liens logiques.

- Gestion Logique des Équipements
Intègre les concepts clés : Routeurs, Switches, Firewalls, Serveurs, Endpoints.
Générateur de “Zones” (DMZ, LAN, WAN) pour le cloisonnement logique.
Chaque équipement possède ses tables de routage et ses interfaces virtuellement éditables à la volée.

- État Persistant & Interopérabilité
Export complet de la topologie (coordonnées XY, configurations, dictionnaire VLAN) en JSON.
Fonctionnalité de Fusion (Merge) : Importez le fichier JSON d’un collègue, l’algorithme calculera automatiquement un offset géométrique pour fusionner sa topologie avec la vôtre sans superposer les éléments.
Print Mode : Génération d’une version épurée en noir et blanc, optimisée pour l’export PDF ou l’impression A3 (Retrait du grid, bordures pleines, couleurs de câbles adaptées).

-  Stack Technique (Under the Hood)
Core : Vanilla HTML5, CSS3, ES6 JavaScript. (Aucun framework JS).
Styling : TailwindCSS (via CDN ou compilé) pour un design System fluide et des thèmes (Dark, Light/Pro, Neutral/VSCode).
Rendering : Manipulation conjointe du DOM (pour les fenêtres et l’interactivité) et du SVG via namespace XML (pour le rendu vectoriel des câbles de bout en bout).
