# Au pays de Candi
Notions de sécurité sur Internet

## Sommaire
1. Préambule
  a. Pourquoi faire ?
  b. Chiffrement, crypate ?
  c. Chiffrement asymétrique ?
  d. Open-source !
  e. Exemple de technique d'attaque
2. Le maillon faible
  a. Choisir un bon mot de passe
  b. Diversifier vos outils
  c. FAI
3.Le maillon fort
  a. Navigation sans surprise
  b. Chiffrer / Signer ses courriels
  c. Truecrypt
  d. Tor
  e. Freenet
  f. I2P
  g. VPN
4. Annexes
  a. Sources
  b. Neutralité du réseau
  c. À propos de la présentation
  d. À propos de l'auteur
  
## Pourquoi faire ?
"Brico 3000, parce qu'on ne sait jamais"
- Droit à la vie privée.
- Rester maître de sa communication.
- Éviter les fuites.
- Protéger l'émetteur ou le destinataire.
- Vous êtes sur écoute.
  
## Chiffrage, cryptage : Quelle différence ?
- Chiffrer : Rendre illisible un texte aux personnes non souhaitées.
- Cryptogramme : Message rendu illisible par chiffrage.
- Crypter : dérive de l'anglais « encryption ».

*Attention différence importante en **déchiffrer et décrypter** !*
- Déchiffrer : Rendre lisible un message chiffré avec la clé de déchiffrement
- Décrypter : Rendre lisible un message chiffré sans la clé de déchiffrement

## Chiffrement asymétrique ?
**Problématique :**
Comment assurer la sécurité d'une communication ?

En mettant au point un code/clé connu uniquement des personnes en relations

**Problématique :**
Comment transmettre ce code de manière sécurisé ?

Génération d'une paire de clé
● Clé publique permettant de chiffrer un contenu

## L'Open source, c'est bien
*Rappel :*
Un logiciel est dit open source si il respecte les règles émises par l'OSI (la redistribution libre, un code source disponible, ...)

- Vous êtes sûr que ce logiciel remplit sa mission, et uniquement sa mission.
- Si vous ne savez pas lire le code, d'autres le feront pour vous.
*Un logiciel open source sans communauté, c'est comme un Windows sans malware.*
- Les failles sont rapidement connues par la communauté puis corrigées.
- Un logiciel de sécurité open source ne repose pas sur le secret pour être efficace, mais bien sur la technique.

## Open Source = Libre ?
**Une différence de philosophie**
### Open Source :
Méthode de développement, aspect pratique pour les développeurs et utilisateurs.
Un logiciel non libre est sous optimale.

### Libre :
Le logiciel non libre est un problème social.
L'aspect pratique n'est que secondaire, ce qui compte c'est la **liberté de l'utilisateur.**
Une philosophie à part entière.

## Méthodes d'attaques
### Man in the middle
Typiquement, c'est ce que fait l'héroïne dans le film « Millenium ». Consiste à écouter les échanges entrants et sortants d'un point.

### Deep Packet Inspection (DPI)
**DANGER DANGER DANGER**
Analyse en profondeur des paquets transitant sur un réseau permettant de lire, analyser, classifier, rediriger, bloquer des contenus. Atteinte à la neutralité du réseau (mais on n'est plus à ça près avec cette technique)

## Utilisateur : le maillon faible
- Le maillon faible se situe entre la chaise et le clavier. (Error type PEBKAC)
- La sécurité reste avant tout un ensemble d'habitudes à prendre, une « hygiène de vie »
- Un outil n'est qu'un outil.
- Vous n'êtes pas un outil, donc réfléchissez et apprenez.

## Quelques règles sur les mots de passes
- Les mots de passes liés à « vous » sont à proscrire (votre nom de jeune fille, dates de naissances etc.). Trop simple à deviner. (ps : « azerty » n'est PAS un mdp) 
- Les « mots » sont à éviter. Facile à forcer avec des attaques de type « dictionnaire » (un logiciel essaye tous les mots d'un dictionnaire ou d'une liste.)
- Idéalement, un mot de passe par application/site.
- Technique pour faire un mot de passe compliqué : « Je m'appelle Bob, et je suis un vrai bonhomme à LoL » → « Jm'aB,ejsuvbàLoL»

### Plusieurs niveaux de mots de passe
- « Léger » - Site peu important, sans risque pour vous. Exemple de mot de passe : Cacahuete32
- « Moyen » - Site important, risque d'usurpation d'identité.
Exemple de mot de passe : #Ban4n3Flambée
- « Dur/Asian level » - Site sensible. Risque important pour vos informations (type bancaire etc.) ou pour vous. Exemple de mot de passe : ~#gfHJéklàm,5»'
- XKCD en a fait un comic très à propos : https://xkcd.com/936/

## Diversifiez (vos outils)
Google n'est pas votre ami, il ne fait pas ça pour la postérité. Utilisez ses services si vous le souhaitez, mais pas uniquement.
A l'heure actuelle, Google en sait plus sur vous que la DCRI (et pourtant la DCRI n'est pas mauvaise).
« Dont be evil » = « Think Different » c'est beau sur le papier, mais dans les faits on en est loin.
Facebook à côté (de Google) c'est les pages jaunes.

### Alternatives possible à Google
- Recherche : Seeks, Duckduckgo, ixquick, bing, yahoo, …
- Maps : OpenStreetMap
- Analytics : Piwik
- Youtube : dailymotion, vimeo, …
- Gmail : Il vous faut vraiment une liste des alternatives à un webmail ?
- L'association Framasoft fait un énorme boulot pour proposer des alternatives à Google, ça ne fait pas de mal d'aller y jeter un oeil ;)

## FAI : Le maillont faible n°2
Votre fournisseur d'accès Internet (F.A.I) est un des points faible du réseau actuel car tout le contenu passe forcément par lui. Il peut donc voir tout l'usage que vous faîtes de votre accès Internet... Sauf si vous chiffrez.
- D'après Science&Vie, il faudrait 24h pour couper 95% des accès Internet en France du fait de la typologie du réseau concentré autour de 5 acteurs majeurs (les 5% restants étant les réseaux universitaires, et FAI associatif.)
- Vous avez un contrat de confiance tacite avec votre FAI. N'hésitez pas à en changer si vous avez un doute sur son intégrité (Qui a dit Orange et sa politique de traçage par défaut ?).
- FAI associatif ?
Internet est par nature décentralisé. Or les gros FAI centralise le réseau. 
Solution ? Faire pleins pleins pleins de petit FAI <3
Mieux vaut 10 FAI qu'un FAI 10x plus gros. Cette philosophie de hippie-geek est contraire au fonctionnement des entreprises, c'est donc principalement sous le statut « d'association » que ces FAI se créent.

## Maillon fort : les outils disponibles
### Pour une navigation sans surprise
Utiliser l'adresse en httpS si disponible. Mettez en place le https sur vos sites, si possible.
- Désactivation de Javascript par défaut, et activation au cas par cas → « No Script » (add-on
Firefox) Vous seriez surpris de voir le nombre de script qui s'exécute sans qu'on le sache.
- Web of Trust (WOT)
Permet de voir la réputation d'un site web, et de donner son avis. Indice à prendre avec des pincettes mais néanmoins utiles.
- Ghostery
Vous permet de voir, en apprendre plus, et bloquer les éléments de traçage présent sur une page web. Très utile.

### Chiffrer ses courriels
Nécessite une paire de clé (cf GPG)
- Signer un mail
Une signature, générée par votre clé privée, est apposée sur le mail prouvant que c'est bien vous qui émettez le mail
- Chiffrer un mail
vous avez besoin de la clé publique du destinataire.

Exemples de solutions logicielles :
- GPG + Thunderbird + Enigmail (add-on Thunderbird)
- GPGTools +Mail (sources)

### Truecrypt
- Génération de disque virtuel crypté.
- Chiffrement de partition.
- Apparaît comme un simple fichier si non déchiffré.
- Système « Chambre secrète » (utile en cas de torture ou demande insistante).

### The Onion Router (TOR)
- Surfer anonymement. (risque potentiel en sortie, à vérifier)
- Contourner la censure.
- Vous entrez au point A, et sortez au point B, en étant passé par les points C, D, E, ...
- Permettre à d'autre de contourner la censure appliquée chez eux.
- Réseau composé de « relais » .
- Chacun peut être relais.
- Possibilité d'être un « point de sortie » sur certains protocole uniquement.
- Plus il y a « d'utilisateur-relais », plus le réseau est rapide

### Freenet
- Un réseau sur le réseau
- Acentralisé
- Chaque utilisateur héberge une partie du réseau (chiffré, et illisible)
- Darknet possible

**Problème :**
- « Peu » d'utilisateurs et/donc peu de contenu à l'heure actuelle
- Lent (ce réseau n'est pas conçu pour la vitesse)

**Bons points :**
- Censure impossible
- Surveillance très (très très très très) compliquée

### Invisible Internet Project (I2P)
- Navigation chiffré.
- Navigation traversant X nombre de relais avant de vous parvenir, masquant votre trace.
- Accès au Web via serveur mandataire.
- Accès au service intra I2P.

### Et les VPN ?
- Anonymat (comme pour TOR, ce n'est pas votre IP en sortie)
- Chiffrement de la navigation entre vous et le VPN
- Contournement des restrictions géographiques
- Vitesses de chargement plus importante que sur TOR à l'heure actuelle (enfin, tout dépend du VPN)

#### Oui mais...
- Vous donnez les pleins pouvoirs à une entreprise (tout passe par leur serveur) si vous n'avez pas un serveur distant à vous. (et si c'est votre serveur, le lien pourra sûrement être fait entre vous et l'IP captée)
- Les serveurs étant souvent basés hors de France, attentions aux législations locales.
- Payant (souvent)

## Sources
- http://www.francoz.net/doc/gpg/[fr]
- http://reflexesecurite.com/general/chiffrage-cryptage-peu-francais/ [fr]
- http://www.gnu.org/philosophy/free-software-for-freedom.fr.html [fr]
- http://fr.wikipedia.org/wiki/Neutralité_du_réseau [fr]
- http://www.truecrypt.org/[fr]
- https://security.ngoinabox.org/fr/[fr]
- https://cryptoanarchy.org/wiki/Main_Page[en]
- https://www.torproject.org/[en]
- http://openpgp.vie-privee.org/[fr]
- https://www.grc.com/sn/SN-041.htm(à propos de TrueCrypt) [en]
- Si vous voulez un VPN, je vous conseille (mais ce n'est que du conseil) :
  - https://www.ipredator.se/ (PirateBay)
  - http://toonux.net/
  
# Neutralité du réseau
Lors de la présentation de quelques méthodes d'attaques, j'ai parlé de neutralité du réseau. N'étant pas le sujet
de cette présentation, j'ai préféré ne pas éclaircir ce point dans la présentation, mais plutôt faire une annexe.
## Définition
La neutralité du Net exclut toute discrimination à l'égard de la source, de la destination ou du contenu de l'information transmise sur le réseau. Ainsi, ce principe garantit que les utilisateurs ne feront face à aucune gestion du trafic internet qui aurait pour effet de limiter leur accès aux applications et services distribués sur le réseau. La neutralité du Net assure que les flux d'information ne sont ni bloqués, ni dégradés, ni favorisés par les opérateurs de télécommunications, permettant ainsi aux utilisateurs d'utiliser librement l'architecture communicationnelle.

## J'ai rien compris.
En profane ça donne :
Le fournisseur d'accès à Internet (FAI) ne doit en aucune manière volontairement dégradé ou empêcher l'accès à un contenu sur le réseau. Le FAI ne doit faire aucune discrimination entre les différentes sources de contenus, et les différents demandeurs de contenu.

## Exemple :
- Orange ne doit pas bridé Spotify pour promouvoir l'accès à Deezer.
- SFR ne doit pas faire d'offre du type « Pour 5€/mois, profite d'un accès plus rapide à Facebook » .
- Free ne doit pas placer de cookie de traçage permettant une publicité ciblée sur les pages demandées par ses utilisateurs.

# À propos de la présentation
J'ai réalisé cette présentation dans le but de sensibiliser et de proposer des solutions pour vivre une vie numérique (plus) sécurisée.
J'ai essayé de garder un discours simple et compréhensible de tous. Cependant, cette présentation fut à l'origine conçu pour n'être qu'un support écrit à un discours oral pour des étudiants en multimédia ayant des connaissances en informatiques. Certains points donc pourront donc être perçu comme obscurs par des néophytes, et je m'en excuse. Google n'est pas votre ami, mais je vous invite à rechercher par vous même sur Internet les réponses à vos questions. 

**Ce document est placé sous licence CC-By.**
La reproduction, l'amélioration et la diffusion sont vivement encouragée.

# À propos de l'auteur
Hey,
Je suis étudiant dans une formation orientée conception de sites web/Gestion de projet, la sécurité personnelle sur le réseau ne fait pas partie de mon coeur de métier (c'est même plutôt le contraire que l'on m'enseigne... Tu aimes le tracking publicitaire ? Mes profs oui.)
Mes connaissances dans le domaine de la sécurité se limite à ce que j'ai pu découvrir au gré de mes pérégrinations sur le réseau et dans les conférences traitant du sujet.
Du fait de cet apprentissage morceau par morceau, il est possible que des notions m'aient échappé entraînant des erreurs d'interprétation. Si c'est le cas, merci de me prévenir afin que je corrige le document « source ».
