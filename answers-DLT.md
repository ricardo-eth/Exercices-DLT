# Exercices Distributed Ledger Technology

- Un arbre de merkle nécessite une paire de hashes pour produire un nouveau hash parent. Il faut donc a absolument que le nombre de transactions qui produiront le `Merkle root` soit pair.  
  Comment est géré le cas ou le nombre de transactions dans le Block à valider est impair pour générer un `Merlke root` ?

  > \*S’il y a un nombre impair de transactions dans le Block, la solution est de dupliquer simplement le dernier hachage pour le rendre pair.\*

- Dans le réseau bitcoin, Comment un nouveau noeud arrive t'il à retrouver ses pairs et ainsi rejoindre le réseau ?

  > \*les nouveaux nœuds peuvent rejoindre le réseau a tout moment, il sufit d'acceptant à leur retour la chaîne de preuve de travail la plus longue (nœud prend part à toutes les opérations réalisées sur le réseau) comme preuve de ce qui s’est déroulé avant la création du nouveau nœud\*

- Pouvez vous nommer au moins une personne qui a ou aurait pu influencer directement ou indirectement la création de Bitcoin par ses travaux (une personne qui n'a pas été nommée dans le cours)?

  > \* - Martti Malmi, vend 5050 bitcoins pour 5,02 $ virés sur son compte Paypal, première vente de bitcoins en dollars - Laszlo Hanyecz, un développeur floridien, expérimente avec succès le minage par GPU (processeur graphique) puis achète deux pizzas pour 10 000 bitcoins.\*

- Avec vos propres recherches et grâce aux compétences acquises en cours pouvez vous expliquer comment une Blockchain crée un lien entre ses différents Blocks?

  > \* Lorsqu’un utilisateur effectue une transaction à travers le réseau blockchain, cette dernière est regroupée avec d'autres transactions au sein d'un bloc. Elle est ensuite vérifiée et validée par des membres du réseau\*

- Quelle structure de données informatique peut représenter le mieux cette chaine de Block: https://en.wikipedia.org/wiki/List_of_data_structures ?

  > \* Les blocs sont similaires aux nœuds d'une Liste chaînée (Linked list), chaque bloc contient plusieurs éléments. Les éléments d'un bloc sont généralement séparés dans l'en-tête du bloc et ses transactions, alors que les transactions dans un bloc représentent la plupart des données, l'en-tête de bloc contient des métadonnées essentielles sur chaque bloc\*

- Si je souhaite modifier une transaction de 10 bitcoin que j'ai effectué il y a 6 mois en une transaction de 1 Bitcoin, que dois je modifier dans la Blockchain et que dois je mettre en oeuvre pour que cette modification persiste ?  
  Est ce possible selon vous ?

  > \*Ce n'est pas possible, car si Alice a envoyé 10 bitcoin à Bob il y a 6 mois, Alice ne peut pas modifier la transation car le block avec la transaction a été validé sur la blockchain qui prouve que Alice a envoyé 10 bitcoin à Bob il y a 6 mois, mais Alice peut toujour créer une nouvelle transation en envoyant à nouveau 1 Bitcoin si elle a assez de bitcoin sur son wallet.\*

  > \*C'est possible mais plutot impossible... car si Alice veut vraiment modifier la transaction il y a 6 mois il faut qu'elle mène une attaque 51 % disposerait de la puissance de minage suffisante pour exclure ou modifier l'ordre des transactions. Alors bonne chance...\*
