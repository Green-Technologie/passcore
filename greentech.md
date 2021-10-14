Ce logiciel a été installé sur GTAP avec quelques modifications.

Deux commits venant d'un fork ont été cherry picked pour que la sélection des groupes dont on peut changer le mot de passe fonctionne bien.

Le site web a été build directement depuis le dernier commit de la branche master.

Les modifications faites dans appsettings.json sont les suivantes :

- Le groupe "Administrators" ne peut pas utiliser le logiciel.
- Le groupe "Domain Users" peut.
- Le domaine par défaut est greentechnologie.net
- Recaptcha a été installé.
- L'email n'est pas utilisé à la place du username.

Le problème du captcha est qu'il semble rester valide après plusieurs utilisations du formulaire mais réellement non, il faut recharger la page à chaque fois.

Pour éteindre PassCore, il faut se connecter à GTAP, aller dans "Services" sur le dossier démarrer, aller tout en bas jusqu'à "World Wide Web Publishing Service" puis faire clic droit et "Stop".
