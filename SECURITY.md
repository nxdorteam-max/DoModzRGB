# Sécurité des mises à jour

Les fichiers `update.json` et `update.sig` sont utilisés par DoModz RGB pour authentifier chaque installateur. La signature RSA-PSS/SHA-256 est vérifiée avec une clé publique intégrée au logiciel ; une empreinte SHA-256 seule ne constitue pas une signature.

Les mises à jour ne récupèrent aucun jeton GitHub et ne nécessitent pas l’accès au dépôt privé. La clé privée n’est jamais intégrée au programme, à l’installateur ou au dépôt public.

La protection contre les versions anciennes compare la version proposée à celle du logiciel installé. L’installation conserve les paramètres et rend les commandes de ventilation au matériel pendant le remplacement des fichiers.

Pour signaler une vulnérabilité, ne publiez pas de jetons, clés, mots de passe ou données personnelles dans un ticket. Utilisez le signalement privé GitHub s’il est disponible ; sinon ouvrez un ticket sans détails exploitables afin de convenir d’un canal privé.
