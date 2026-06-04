Californie, 1969. Un tueur en série se faisant appeler « Le Zodiaque » terrorise la population. Il revendique ses crimes dans des lettres chiffrées qu’il envoie ensuite aux médias ainsi qu’aux forces de l’ordre. Cinquante ans plus tard, son identité reste inconnue, mais certains de ces codes, eux, ont fini par parler.

Quatre lettres : Z408, Z340, Z32 et Z13. Des symboles, triangles, cercles barrés, lettres grecques, signes astrologiques.. Un vrai charabia visuel.

# Le bon code n’est pas l’incassable

En cybersécurité, on entend constamment parler de chiffrement “militaire”, de cryptographie “post-quantique”, de protocoles “inviolables”. La vraie question opérationnelle n’est finalement jamais “est-ce incassable ?”, mais, “combien de temps ça peut tenir ?”.

L’affaire du Zodiaque offre un terrain d’étude inégalé pour comprendre cette nuance. Un chiffre amateur, conçu par un homme sans formation cryptographique, a tenu en échec les meilleurs services de renseignement pendant des dizaines d’années. Pas parce qu’il était mathématiquement parfait (il ne l’était pas), mais parce qu’il combinait juste assez d’astuces pour décourager les outils de son époque.

# L’astuce du XVIe siècle qui a coûté la tête a une reine
Le Zodiaque n’a rien inventé, il a en réalité réutilisé une technique vieille de 4 siècles : le chiffre de substitution homophonique.

Le principe est simple. Dans un chiffrement classique, chaque lettre est remplacée par un symbole unique (exemple : la lettre “E” deviendra toujours un triangle). Problème, la lettre “E” est une lettre très fréquente en Anglais comme en Français. N’importe qui peut compter les triangles, voir qu’ils dominent et reconstituer le message par analyse de fréquence (technique fondatrice de la cryptanalyse par le savant arabe Al-Kindi au IXe siècle).

Le chiffre homophonique contourne ce piège. Gardons notre exemple de la lettre “E”, cette dernière peut être représentée par 5, 6 ou 10 symboles différents choisis au hasard à chaque occurrence. Grâce à cette technique les variations sont donc atténuées.

# Marie Stuart, 1586 : le premier code homophonique de l’histoire à faire la une
L’usage le plus retentissant de cette technique remonte à la fin du XVIe siècle. Marie Stuart, reine d’Ecosse est emprisonnée en Angleterre. Elle communique avec des partisans afin de renverser sa cousine Elisabeth I. Pour cela, aucun mystère ici, elle utilise un chiffre homophonique. Chaque lettre dispose de plusieurs symboles, complétés par un répertoire de mots-codes pour les noms et expressions sensibles.

Grâce à un système de chiffrage dit “homophonique”, chaque lettre de l’alphabet est représentée par plusieurs symboles.

Marie se croyait protégée. Elle ne l’était pas.

Francis Walsingham, le maître espion d’Elisabeth, avait infiltré toute la chaîne de transmission. Son cryptanalyste, Thomas Phelippes, a cassé le code par analyse de fréquence combinée à la méthode du mot probable (formalisée par le cryptographe italien Giambattista della Porta), il devinait les noms qui devaient figurer dans une correspondance conspirative. Les lettres déchiffrées ont servi de preuves au procès. Le 8 Février 1587, Marie Stuart est décapitée.

Le chiffre homophonique venait de connaître son premier échec. Le Zodiaque allait répéter l’erreur, mais en y ajoutant quelques astuces.

# Le piège du Z340 : Ajouter du chaos au-dessus de l’astuce
Sur son premier message, le Z408, le Zodiaque s’est contenté du chiffre homophonique classique. Un couple d’enseignants, Donald et Bettye Harden ont réussi à le casser en 8 jours en pariant sur la psychologie humaine. “Quel premier mot utiliserait un tueur en série assez égocentrique pour envoyer ses actes écrits dans des lettres aux médias et forces de l’ordre ?”. La réponse était simple : “I”, “Je”. Sur le Z340, le tueur du Zodiaque avait compris la leçon et empilé 3 couches supplémentaires.

Z340, lettre-cryptogramme du tueur du Zodiaque envoyée au San Francisco Chronicle en novembre 1969.

Première couche : la fragmentation. Le texte n’était pas écrit en continu mais découpé en 4 blocs distincts (2 blocs de 9 lignes, puis 2 bloc d’une ligne chacun) avec un système de chiffrement qui changeait subtilement d’un bloc à l’autre.

Deuxième couche : la lecture en diagonale. Pour reconstituer le message dans l’ordre, il fallait partir du coin supérieur gauche et avancer en décalant d’une case vers le bas et de deux vers la droite à chaque pas.

Troisième couche : les incohérences volontaires. Le Zodiaque a introduit ce qu’on appelle aujourd’hui du bruit (écarts par rapport à ses propres règles qui faisaient échouer toute tentative de décodage systématique).

Aucune de ces astuces n’est mathématiquement sophistiquée mais combinées elles ont saturé toutes les approches algorithmiques disponibles dans les années 70, 80, 90 et 2000.

# Quand la puissance de calcul change la donne
Décembre 2020. Trois hommes répartis sur trois continents voient AZdecrypt sortir trois phrases qui sautent aux yeux dans le résultat : HOPE YOU ARE, TRYING TO CATCH ME, GAS CHAMBER. Le 5 décembre 2020 ils transmettent la solution au FBI.

Ce qui a fait basculer l’affaire, c’est l’accumulation de 2 choses :

Un logiciel spécialisé, AZdecrypt, développé par Jarl Van Eycke spécifiquement pour les chiffres de substitution homophoniques

La puissance de calcul d’un ordinateur personnel moderne, capable de tester des millions d’hypothèses de lecture par seconde.

Il est possible de retrouver l’intégralité de cette méthode (dans ce papier) documentée par le trio à son origine (Oranchack/Blake/Van Eycke)

Le contenu du message est le suivant :

“J’espère que vous vous amusez bien en essayant de m’attraper. Ce n’était pas moi à la télévision, ce qui m’amène à dire quelque chose sur moi : je n’ai pas peur de la chambre à gaz car elle m’enverra plus tôt au paradis parce que j’ai maintenant assez d’esclaves pour travailler pour moi alors que tous les autres n’ont rien quand ils arrivent au paradis : c’est pour ça qu’ils ont peur de la mort. Je n’ai pas peur car je sais que ma nouvelle vie sera facile dans l’au-delà, au paradis”

Message presque décevant faisant référence à une émission de télévision AM San Francisco de Jim Dunbar, diffusée sur KGO-TV en octobre 1969, dans laquelle un homme prétendait être le tueur, et la promesse d’un paradis peuplé d’esclaves. Aucune révélation, aucun nom.

Deux autres messages restent à ce jour non résolus : le Z32, qui prétendait localiser une bombe sous un bus scolaire (envoyé en juin 1970) et le Z13, 13 lettres qui prétendent donner le nom du tueur.

Le message codé Z13 écrit et transmis par le tueur du Zodiac qui donnerait son nom.

Le Z340 n’était pas incassable. Il a juste tenu plus de 50 ans, ce qui, pour son autour était bien suffisant.

# Trois leçons que le Zodiaque laisse en héritage
Sur le plan technique. Dans leur papier, Oranchack, Blake et Van Eycke, expliquent que le Zodiaque a réussi à appliquer le principe de la sécurité par l’obscurité : l’ignorance de la présence et des composants d’une méthode de secret suffit à protéger ce secret. Ils ajoutent aussi que si le Zodiaque avait utilisé un système classique bien compris (substitution homophonique seule, transposition seule..) la cryptanalyse traditionnelle aurait cassé son chiffre rapidement. Ce qui l’a sauvé, c’est l’empilement de petites complications inhabituelles. Ils se permettent même de préciser que si le Zodiaque avait ajouté ne serait-ce qu’une couche supplémentaire, son chiffre serait probablement encore non résolu aujourd’hui. C’est un constat qui contredit en pratique le principe de Kerckhoffs, règle d’or de la cryptographie moderne qui veut qu’un bon système reste sûr même si l’ennemi en connaît tous les rouages, à l’exception de la clé. Pour nuancer, il ne faut jamais se reposer sur l’obscurité comme défense principale, mais ne jamais l’ignorer comme couche complémentaire.

Sur le plan humain. L’histoire du Z340 illustre une asymétrie fondamentale entre attaquant et défenseur. Le Zodiaque n’a pas passé le même nombre d’heures à concevoir son chiffre alors que le FBI a mobilisé une équipe entière pendant plus de 50ans. Cette asymétrie temporelle joue presque toujours en faveur du défenseur un peu paresseux. C’est ce qui explique que tant de systèmes informatiques bricolés dans les années 90 encore en prod aujourd’hui restent fonctionnellement sécurisés non pas par leur robustesse, mais parce que personne n’a investi le temps nécessaire afin de les analyser sérieusement.

Sur le plan métier. Pour un pentester ou un professionnel de la sécurité offensive, la leçon est opérationnelle : la première étape d’une attaque réside toujours dans l’identification du type de système. Tant qu’on n’a pas correctement identifié à quel type de système on a affaire, toutes les attaques sont aveugles.
