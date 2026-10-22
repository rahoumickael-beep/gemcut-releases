# Gemcut — version bêta

Gemcut repère les meilleurs moments de tes parties (League of Legends, Counter-Strike 2…) et te prépare des Shorts
prêts à valider, puis à publier. Tes vidéos restent sur ton PC.

Merci de tester cette bêta ! Ce guide t'accompagne de l'installation au premier Short.

**[⬇️ Télécharger Gemcut 1.0.4 (Windows, 107 Mo)](https://github.com/rahoumickael-beep/gemcut-releases/releases/download/v1.0.4/Gemcut_Setup_1.0.4.exe)**

---

## Avant de commencer

| | |
|---|---|
| **Système** | Windows 10 ou 11, 64 bits (testé sur Windows 11) |
| **Espace disque** | environ 8 Go pour Gemcut, et 20 Go libres conseillés pour tes vidéos |
| **Internet** | nécessaire pendant l'installation : Gemcut télécharge ses composants d'IA |
| **Carte graphique** | une carte NVIDIA accélère tout, mais elle n'est pas obligatoire |
| **Conseillé** | [Outplayed](https://www.overwolf.com/app/overwolf-outplayed) pour enregistrer tes parties |

Compte **15 à 30 minutes** pour l'installation, selon ta connexion.

## 1. Installer

1. Ouvre `Gemcut_Setup_1.0.4.exe`.
2. Ton navigateur peut te prévenir que ce fichier est **rarement téléchargé** : choisis de le conserver.
3. Windows peut afficher un écran bleu **« Windows a protégé votre ordinateur »**. C'est normal pour une bêta qui
   n'a pas encore de signature numérique : clique sur **Informations complémentaires**, puis sur **Exécuter quand même**.
4. Aucun droit administrateur n'est demandé : Gemcut s'installe seulement pour ton compte Windows.
5. Pendant la configuration (15 à 30 min), **ne ferme pas la fenêtre**, même si elle semble immobile.
6. À la fin, laisse cochée la case **Exécuter Gemcut**.

> **Si Windows 11 affiche « Le Contrôle intelligent des applications a bloqué… »**, il n'y a pas de bouton pour
> continuer. Ne désactive pas cette protection : préviens la personne qui t'a invité à la bêta.

**Si l'installation échoue**, une fenêtre te le dit, et Gemcut ne se lance pas. Envoie le journal à la personne qui
t'a invité à la bêta. Il se trouve ici (copie-colle cette ligne dans l'Explorateur) :

```
%LOCALAPPDATA%\Gemcut\data\logs\installation.log
```

Tu peux ensuite relancer l'installateur.

## 2. Premier lancement

Gemcut s'ouvre sur un accueil en **5 étapes** :

1. **Bienvenue**.
2. **Ton PC est-il prêt ?** : Gemcut vérifie ton PC (vidéo, Outplayed, OBS, voix…) et te dit quoi régler.
   Rien n'est installé sans toi.
3. **D'où viennent tes streams ?** : Outplayed, OBS, un fichier vidéo ou Twitch.
4. **Ton premier import** : choisis une vidéo.
5. **Analyse** : tu peux terminer sans attendre, l'analyse continue en arrière-plan. Les moments forts arrivent dans
   **Pépites**.

Tu peux t'arrêter avec **Plus tard** et reprendre quand tu veux : Réglages › Général › **Revoir la présentation de départ**.

## 3. Activer l'IA en ligne (gratuit)

Les titres, les idées et les réponses de l'assistant utilisent ta propre clé **Groq**, gratuite.

1. Dans Gemcut : **Réglages › Comptes connectés**, carte **IA en ligne (Groq)**, bouton **Obtenir une clé**.
2. Sur [console.groq.com/keys](https://console.groq.com/keys), crée un compte puis une clé. Elle commence par `gsk_`.
3. De retour dans Gemcut : **Ajouter ma clé**, colle-la, **Enregistrer**, puis **Tester**.

Ta clé est chiffrée sur ton PC et n'est jamais réaffichée. Seuls de courts textes partent vers Groq (titres, phrases
dites à l'assistant…). Aucune vidéo, aucun son.

## 4. Commande vocale (facultatif)

Elle est **coupée par défaut** : Gemcut n'écoute pas ton micro. Pour l'essayer : **Réglages › Voix › Commande vocale**.
Tout est transcrit sur ton PC. Sans carte NVIDIA, l'écoute utilise ton processeur pendant que tu joues.

## 5. Un souci ? Envoie un rapport

**Réglages › À propos › Créer un rapport pour l'équipe** : Gemcut crée un fichier `Gemcut-rapport-….zip` sur ton
Bureau. Envoie-le à la personne qui t'a invité à la bêta.

Rien n'est envoyé tout seul. Le rapport contient les journaux de Gemcut et une fiche de ton matériel (processeur,
mémoire, carte graphique, version de Windows). Tes clés, tes mots de passe, ton adresse e-mail et ton nom d'utilisateur
Windows en sont retirés.

## Mises à jour

Gemcut vérifie s'il existe une nouvelle version au démarrage, puis toutes les 6 heures. Il la télécharge en arrière-plan
et l'installe **quand tu fermes Gemcut**. Jamais pendant une partie, un stream ou un rendu.

## Ce qui reste sur ton PC, ce qui part en ligne

- **Sur ton PC** : tes enregistrements, tes vidéos et leurs transcriptions, tes identifiants (chiffrés).
- **En ligne, seulement si tu t'en sers** : les publications vers les comptes que tu connectes ; de courts textes vers
  Groq si tu as mis une clé.
- **Voix de l'assistant** : par défaut, les phrases que Gemcut prononce sont fabriquées par le service vocal en ligne de
  Microsoft. Hors ligne, une voix locale prend le relais.
- **Automatiquement** : la vérification des mises à jour, et une veille des sujets tendance (flux publics comme Google
  Trends et Reddit).

## Désinstaller

Paramètres de Windows › **Applications › Applications installées** › **Gemcut** › **Désinstaller**.

Tes vidéos (`Vidéos\Gemcut`) et tes réglages (`%LOCALAPPDATA%\Gemcut`) sont conservés. Supprime ces dossiers à la main si
tu veux tout effacer.
