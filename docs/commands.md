# 🤖 Commandes du Bot Modmail

## 📑 Table des matières
- [📨 Dans un fil Modmail](#dans-un-fil-modmail)
- [🌐 Partout sur le serveur de réception](#partout-sur-le-serveur-de-réception)
- [📋 Modèles de réponses (Snippets)](#modèles-de-réponses-snippets)

---

## 📨 Dans un fil Modmail

Ces commandes ne peuvent être utilisées que dans un canal de fil Modmail sur le serveur de réception.

### `!reply <texte>` / `!r <texte>`
Répond à l'utilisateur.  
**Exemple :** `!r Comment puis-je vous aider ?`  
Pour répondre automatiquement sans utiliser `!reply`, [activez `alwaysReply` dans les paramètres du bot](configuration.md).

### `!anonreply <texte>` / `!ar <texte>`
Envoie une réponse **anonyme** (seul le rôle du modérateur est visible).  
**Exemple :** `!ar Merci d'utiliser Modmail uniquement pour des messages sérieux`

### `!realreply <texte>` / `!rr <texte>`
Répond à l'utilisateur en **affichant toujours le nom du modérateur**, même si `forceAnon` est activé.

### `!close`
Ferme le fil de discussion.

### `!close <durée>`
Ferme le fil après un délai défini.  
**Exemple :** `!close 15m` (ferme dans 15 minutes)  
L’envoi ou la réception d’un message annule cette fermeture programmée.

### `!close -s` / `!close -s <durée>`
Ferme le fil **silencieusement** (l'utilisateur n'est pas informé).

### `!close cancel`
Annule une fermeture programmée.

### `!logs`
Affiche les anciens logs avec cet utilisateur.

### `!block`
Bloque l'utilisateur de Modmail.

### `!block <durée>`
Bloque l’utilisateur pour une durée définie.  
**Exemple :** `!block 7d` (7 jours)

### `!unblock`
Débloque l’utilisateur.

### `!move <catégorie>`
Déplace le fil vers une autre catégorie.  
Nécessite l’activation de `allowMove` dans les paramètres.

### `!suspend`
Suspend temporairement le fil. Aucun message ne sera reçu jusqu’à reprise avec `!unsuspend`.

### `!unsuspend`
Réactive un fil suspendu.

### `!alert`
Vous notifie quand une nouvelle réponse arrive dans le fil.

### `!alert cancel`
Annule l’alerte.

### `!edit <numéro> <nouveau texte>`
Modifie une ancienne réponse.  
`<numéro>` = numéro du message à modifier (visible dans le fil).

### `!delete <numéro>`
Supprime une réponse précédente.

### `!role`
Affiche votre rôle d'affichage pour ce fil.

### `!role reset`
Réinitialise votre rôle d'affichage.

### `!role <nom du rôle>`
Définit votre rôle d'affichage à un rôle que vous possédez.

### `!loglink`
Fournit un lien vers les logs du fil actuel.

### `!loglink -s`
Lien des logs **sans les discussions entre modérateurs**.

### `!loglink -v`
Lien des logs **détaillés** (ID des messages, utile pour signaler à Discord).

### `!id`
Affiche l'identifiant de l'utilisateur.

### `!note <texte>`
Ajoute une note pour l'utilisateur.

### `!notes <userID>`
Affiche toutes les notes liées à cet utilisateur.

### `!delete_note <noteID>`
Supprime une note spécifique.

### `!dm_channel_id`
Affiche l’ID du canal de messages privés avec l’utilisateur.

### `!message <numéro>`
Affiche l'ID du canal MP, l’ID du message et un lien vers ce message.

---

## 🌐 Partout sur le serveur de réception

Ces commandes fonctionnent **en dehors** des fils Modmail, n'importe où sur le serveur.

### `!newthread <userID>`
Ouvre un nouveau fil avec un utilisateur.  
**Exemple :** `!newthread 106391128718245888`

### `!logs <userID>`
Affiche les anciens logs de cet utilisateur.

### `!block <userID>`
Bloque cet utilisateur.

### `!block <userID> <durée>`
Bloque cet utilisateur pour une durée définie.  
**Exemple :** `!block 106391128718245888 7d`

### `!unblock <userID>`
Débloque cet utilisateur.

### `!is_blocked <userID>`
Vérifie si un utilisateur est bloqué.

### `!role`
Affiche votre rôle d'affichage par défaut.

### `!role reset`
Réinitialise votre rôle d'affichage par défaut.

### `!role <nom du rôle>`
Définit un nouveau rôle d'affichage par défaut.

### `!note <userID> <texte>`
Ajoute une note à un utilisateur.

### `!notes <userID>`
Affiche les notes d’un utilisateur.

### `!delete_note <noteID>`
Supprime une note via son identifiant.

### `!version`
Affiche la version du bot Modmail.

---

## 📋 Modèles de réponses (Snippets)

Voir la page [📋 Snippets](snippets.md) pour plus d’informations.
