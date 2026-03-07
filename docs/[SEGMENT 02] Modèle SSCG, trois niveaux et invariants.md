[SEGMENT 02] Modèle SSCG, trois niveaux et invariants

SSCG impose une rupture en trois couches. Ce qui est écrit, ce qui est montré au LLM, ce qui existe réellement. Ces trois espaces ne se recoupent jamais.

N0 est la matière brute. Noms d'utilisateurs, chemins absolus, adresses IP, identifiants de services. Ce niveau est lisible, directement exploitable. Il ne sort pas du moteur local. Tant qu'un élément reste en N0, il n'existe pas dans l'espace du modèle.

N1 efface le système. Chaque élément de N0 est remplacé par un identifiant arbitraire, HGt56, Q9xA1, Cq8Gg, Nm4Zz. Pas des alias. Pas des abréviations. Des marqueurs sans structure exploitable, sans préfixe porteur de sens, sans hiérarchie lisible. Un chemin et un port produisent des tokens visuellement indiscernables. Toute corrélation directe avec le système réel s'arrête ici.

N2 ajoute une sémantique fonctionnelle sur ces tokens opaques. HGt56 devient IDENTITY_ROOT. Cq8Gg devient PATH_HOME_USER_PRIMARY. Rj1Qq devient NTP_SERVER_DISTRO_DEFAULT. On ne revient pas vers le réel, on construit un vocabulaire de rôles dans un OS générique. C'est uniquement ce vocabulaire que le LLM reçoit. Il manipule des fonctions. Jamais des instances.

Trois invariants encadrent ces transitions.

La traduction N0 → N1 est unidirectionnelle et locale. Aucune structure de N0, format, préfixe, hiérarchie , ne transite dans les tokens. Un adversaire avec accès complet à N1 ne reconstruit pas N0 sans le traducteur.

La traduction N1 → N2 est stable, mais non injective sur le réel. Plusieurs éléments réels peuvent occuper le même rôle sémantique. Un rôle peut être réassigné sans que le modèle en détecte le changement.

N2 ne contient aucune donnée brute. Aucune adresse, aucun chemin, aucun hostname, aucune clé. Ce qui ressemble à une valeur est ramené à un type, une catégorie, un rôle. Toute exception constitue une fuite.

Le moteur local est le seul composant à connaître N0. Il reçoit les requêtes du LLM formulées en N2, les résout vers N1 puis vers l'OS, et vérifie les invariants avant chaque action. Une commande qui viole ces contraintes est rejetée ou réécrite. Aucune remontée d'information dans ces cas. L'espace N2 reste intact.

SSCG.txt n'est pas un fichier de configuration. C'est la matérialisation de l'espace N1 → N2 : un vocabulaire suffisamment riche pour décrire un OS complet sans laisser fuiter un seul élément de sa structure réelle. Le LLM opère dans cet espace. Il n'en sort jamais.

Le segment suivant couvre le comportement opérationnel de cette architecture,  ce qui se passe à l'exécution, et les conditions dans lesquelles le modèle cesse d'être valide.
