::: {custom-style="Cover Title"}
Vérif'IA
:::

::: {custom-style="Cover Subtitle"}
Avant de croire. Avant de partager. Vérifiez.
:::

::: {custom-style="Cover Text"}
**Projet IA – Désinformation et intelligence artificielle** · EFAP · Octobre 2026

**Challenge n° 1 :** Repérer une fausse information avant qu'elle ne devienne virale

**Groupe 9 :** Hiba Gherraby · Shems Mrini · Eugenia Colmenares · Olivia Clerico · Ngoc Nhi Luu

**Maquette cliquable :** <https://verifia-efap.vercel.app>
:::

**Vérif'IA en une phrase.** Pour les lycéens qui partagent une vidéo choc à leurs amis avant d'avoir pu la vérifier, nous créons Vérif'IA, un assistant virtuel intégré au bouton « Partager », qui leur indique en 10 secondes si un contenu est douteux et pourquoi, grâce à une IA qui analyse le contenu, son origine et sa diffusion, contrairement au fact-checking classique, qui arrive quand la rumeur est déjà virale.

**Sommaire**

1. Le challenge
2. La cible et les personas
3. L'insight
4. L'existant et ce qui manque
5. Notre solution : Vérif'IA
6. La maquette
7. L'IA et les garde-fous
8. Impact et déploiement
9. Notre usage de l'IA pour construire le projet

L'équipe

```{=openxml}
<w:p><w:r><w:br w:type="page"/></w:r></w:p>
```

# 1. Le challenge

**Challenge n° 1 : Repérer une fausse information avant qu'elle ne devienne virale.**

Aujourd'hui, une information peut être partagée des milliers de fois en quelques minutes sur les réseaux sociaux et les messageries. Et le faux circule plus vite que le vrai : selon une étude du MIT publiée dans la revue *Science* en 2018, une fausse information a 70 % de chances de plus d'être repartagée qu'une vraie. Quand le démenti arrive, la rumeur a souvent déjà fait le tour des groupes.

Notre réflexion part d'un constat simple : on partage souvent une information avant même d'avoir eu le temps de vérifier si elle est vraie. C'est le cercle vicieux de la désinformation :

> Je reçois une information → je la trouve crédible → je la partage → quelqu'un d'autre la reçoit → il la partage à son tour → l'information devient virale.

Le problème n'est donc pas seulement de détecter une fausse information, mais d'intervenir au bon moment : juste avant qu'elle ne se propage.

**Notre problématique :** comment utiliser l'intelligence artificielle pour aider chacun à repérer une fausse information au moment où il s'apprête à la partager, avant qu'elle ne devienne virale ?

# 2. La cible et les personas

**Cible principale : les lycéens de 15 à 17 ans.** C'est avec eux que nous lançons le pilote. Ils consomment énormément de contenus courts, les partagent vite entre amis, et nous pouvons les atteindre facilement grâce aux lycées et aux ateliers d'éducation aux médias.

## Persona principal : Léa, 16 ans, « la très connectée »

![Léa, 16 ans (image générée par IA)](images/lea.jpg){width=3.2cm}

- **Situation :** lycéenne.
- **Habitudes numériques :** utilise surtout TikTok, Snapchat et Instagram, ainsi que les messageries ; consomme principalement des contenus courts ; suit des influenceurs et des créateurs de contenu ; partage facilement des vidéos ou des captures d'écran avec ses amies.
- **Problème :** elle reçoit énormément d'informations, mais ne sait pas toujours distinguer une information, une opinion, une rumeur ou une fake news.
- **Besoin principal :** « Je veux savoir rapidement si ce que je vois est vrai. »
- **Le moment critique :** le soir, sur son téléphone, quand une vidéo choc circule déjà dans le groupe de ses amies et qu'elle n'a que quelques secondes pour décider de l'envoyer ou non.
- **Ce que lui apporte Vérif'IA :** une vérification très simple, visuelle et ludique, en 10 secondes, là où elle partage déjà.

## Les cibles secondaires

Les trois autres personas représentent les publics que Vérif'IA touchera dans un second temps (voir partie 8).

: Tableau 1 – Les cibles secondaires

| Persona | Profil et habitudes | Problème | Besoin | Quand nous l'atteignons |
|:-----------|:------------------|:------------------|:----------------|:-------------|
| **Nathalie, 44 ans** – le relais familial | Active ; Facebook et WhatsApp ; très présente dans les groupes familiaux ; reçoit et transfère beaucoup de messages | Reçoit des messages du type « Attention, faites circuler ! » ou « Une personne du secteur m'a confirmé que… », sans savoir comment les vérifier | « Je veux être rassurée avant de transmettre une information à ma famille. » | Phase 3 du pilote : parents d'élèves, ateliers en médiathèque, vidéos « Le Groupe Famille » |
| **Michel, 58 ans** – l'utilisateur prudent | Facebook et WhatsApp ; suit l'actualité ; fait davantage confiance à ce qui vient d'un proche | Une information transmise par un proche lui semble automatiquement crédible | « Je veux un moyen très simple de savoir si ce message est fiable. » | Phase 3 du pilote : ateliers en médiathèque (seniors) |
| **Thomas, 31 ans** – l'actif surinformé | Actif ; LinkedIn, Instagram, Facebook et WhatsApp ; membre de plusieurs groupes WhatsApp | N'a pas le temps de tout vérifier ; une fausse information peut lui nuire dans sa vie professionnelle ou personnelle | « Je veux savoir rapidement si une information est assez fiable pour la transmettre. » | Après le pilote : ouverture aux jeunes actifs (rentrée 2027) |

# 3. L'insight

> **« Dans mon groupe, être la première à partager une info, c'est être dans le coup. Mais si elle est fausse, c'est moi qui passe pour la naïve. »**

Léa ne partage pas une rumeur parce qu'elle est crédule, mais parce que partager vite donne un statut dans son groupe d'amies. Lui demander simplement de « ralentir » ne fonctionne donc pas. Vérif'IA ne lui retire pas ce statut : il le déplace. Être celle qui vérifie en premier, et qui prévient ses amies, devient la nouvelle façon d'être dans le coup.

Cet insight guide tout le projet : l'emplacement de l'outil (le bouton « Partager », là où elle décide), le badge qui récompense les bonnes habitudes, et la campagne de lancement « Vérifie en premier » (partie 8).

# 4. L'existant et ce qui manque

Des solutions existent déjà, mais elles interviennent souvent trop tard, ou ne sont pas conçues pour une lycéenne qui a 10 secondes pour décider.

: Tableau 2 – Les solutions existantes et leurs limites

| Solution existante | Ce qu'elle fait bien | Sa limite pour Léa |
|:---------------------|:---------------------|:-----------------------------|
| Médias de fact-checking (AFP Factuel, Les Décodeurs du *Monde*) | Des vérifications fiables, sourcées et détaillées | Il faut aller les chercher ; l'article arrive souvent quand la rumeur est déjà virale |
| Notes de la communauté (Community Notes sur X) | Du contexte ajouté par les utilisateurs eux-mêmes | La note s'affiche souvent après le pic de diffusion, et sur une seule plateforme |
| Mention « Transféré plusieurs fois » sur WhatsApp | Signale qu'un message circule beaucoup | Ne dit pas si le message est faux, ni pourquoi |
| Chatbots d'IA généralistes (ChatGPT, Le Chat…) | Répondent à n'importe quelle question | Il faut copier le contenu ailleurs et savoir quoi demander ; pas d'indice de fiabilité ni de sources systématiques ; risque d'erreur |
| Outils de vérification pour journalistes (InVID-WeVerify) | Une analyse poussée des images et des vidéos | Trop techniques pour le grand public |

Le fact-checking classique suit cette chronologie : **fausse information → diffusion → viralité → démenti**. Personne n'est présent au moment où tout se joue : le moment du partage. Vérif'IA intervient précisément là : **information → doute → vérification → décision de partager ou non**. Notre ambition est de prévenir la viralité plutôt que d'en corriger seulement les conséquences.

# 5. Notre solution : Vérif'IA

## Le nom et la big idea

**Vérif'IA** associe « vérifier » et « IA » : le nom dit exactement ce que fait l'outil.

**Notre big idea :** un assistant virtuel intégré au bouton « Partager ». Au moment précis où l'on s'apprête à envoyer un contenu, on peut le vérifier en 10 secondes.

**Notre promesse :** « Avec Vérif'IA, tu sais en 10 secondes si un contenu est douteux, et pourquoi, avant de l'envoyer à tes amis. »

Nous ne voulons pas créer un simple « détecteur de fake news » : notre objectif est de créer **un réflexe de vérification**.

## Comment ça marche

Vérif'IA apparaît dans le menu « Partager » du téléphone, à côté des contacts, quand on veut envoyer un contenu depuis TikTok, Instagram ou WhatsApp. On peut aussi lui transmettre directement un texte, un lien, une capture d'écran, une image ou une vidéo.

1. **L'utilisateur transmet le contenu :** au lieu de l'envoyer directement, il appuie sur « Vérifier avec Vérif'IA ».
2. **L'IA analyse le contenu** en quelques secondes : ce qu'il affirme, son origine, sa diffusion, et ce qu'en disent les sources fiables.
3. **Vérif'IA donne un résultat clair :** un indice de fiabilité sur 100, un niveau parmi trois (**Fiable**, **Douteux** ou **Probablement faux**) et les indices qui justifient ce résultat. Chaque indice peut être expliqué (« Pourquoi ? ») ou contesté.
4. **L'utilisateur décide :** ne pas envoyer, prévenir ses amis avec un message préparé par l'IA, ou envoyer quand même.

Vérif'IA ne dit jamais qu'une information est vraie ou fausse à 100 %, car personne ne peut en être sûr. Il ne bloque et ne supprime rien : il ajoute de l'information, et c'est l'utilisateur qui décide.

> **Le parcours vers un partage responsable :** je reçois une information → je doute → je vérifie → je comprends → je décide de partager ou non.

**Exemple.** Un message circule : « À partir de janvier, WhatsApp deviendra payant pour tous les utilisateurs. Partage ce message à tes contacts ! » Vérif'IA répond : **Probablement faux – indice de fiabilité : 15/100.** Pourquoi ? Aucune source officielle identifiée ; information non confirmée par des sources fiables ; formulation alarmiste ; incitation à partager rapidement. L'objectif n'est pas seulement de dire « vrai » ou « faux », mais de faire comprendre pourquoi une information est suspecte.

## Ce qui nous différencie

- **Le moment :** nous intervenons au moment du partage, avant la viralité, et non après.
- **L'explication :** un indice et des raisons claires, pas un simple verdict.
- **Le réflexe :** un badge qui récompense les bonnes habitudes (vérifier, ne pas transférer un contenu douteux, prévenir ses proches), pas le fait d'avoir « raison ».

# 6. La maquette

**Lien :** <https://verifia-efap.vercel.app> (maquette cliquable, à ouvrir sur ordinateur ou sur téléphone ; les données sont fictives).

Le tableau ci-dessous suit le parcours de Léa : ce qu'elle voit, et ce qu'elle fait.

: Tableau 3 – Le parcours de Léa en six écrans

| Écran | Ce que voit Léa | Ce que fait Léa |
|:-------------|:------------------------------------|:----------------------|
| **1. Le moment du doute** | À 21 h 14, une vidéo choc sur TikTok : « Incendie géant gare de Lyon », 1,2 million de vues. Ses amies en parlent déjà dans leur groupe. | Elle appuie sur « Partager » et choisit « Vérifier avec Vérif'IA », à côté de ses contacts. |
| **2. L'analyse** | En quelques secondes, l'IA recherche la première publication, compare la vidéo à des milliers de posts similaires, analyse les comptes qui la diffusent et vérifie l'origine de l'image. | Elle attend une dizaine de secondes. |
| **3. La fiche de vérification** | Indice de fiabilité de 15/100, niveau « Probablement faux », et quatre indices classés du plus fort au plus faible : une image très proche d'une photo publiée en 2021 ; une diffusion qui semble coordonnée (214 comptes publient le même texte en 18 minutes) ; aucune source fiable pour l'instant ; une information de moins d'une heure. Le chemin de la vidéo montre comment elle est arrivée jusqu'à elle. | Elle touche « Pourquoi ? » pour comprendre un indice (ou le conteste), puis choisit : ne pas envoyer, prévenir ses amies ou envoyer quand même. |
| **4. Prévenir ses amies** | Un message rédigé par l'IA à partir de la fiche. | Elle le modifie, joint le résultat et affiche son badge Vérif'IA. |
| **5. Dans la discussion** | Ses amies reçoivent le message et peuvent ouvrir le résultat pour voir les indices. L'une d'elles répond qu'elle allait publier la vidéo en story. | Au lieu de faire circuler la rumeur, Léa l'a arrêtée. |
| **6. Le badge Vérif'IA** | Son niveau (Bronze, Argent, Or), calculé uniquement sur ses habitudes, et un petit défi entre amies. | Elle progresse : se tromper ne fait pas perdre de points, se corriger en fait gagner. |

# 7. L'IA et les garde-fous

Vérif'IA lutte contre la désinformation : il doit donc être lui-même digne de confiance. Une question guide cette partie : qui sommes-nous pour juger un contenu ?

## 7.1. Ce que fait l'IA

- **Comprendre le contenu :** identifier ce que l'information affirme réellement et ce qui peut être vérifié.
- **Comparer aux sources fiables :** vérifications déjà publiées par les fact-checkeurs, médias, institutions et sites officiels.
- **Repérer les signaux de manipulation :** titre sensationnaliste, vocabulaire alarmiste, urgence (« Partage vite ! »), absence de source, faux expert, chiffres suspects, information sortie de son contexte.
- **Analyser les images et les vidéos :** image ancienne réutilisée, image modifiée ou générée par IA. C'est un indice parmi d'autres, jamais une preuve à lui seul.
- **Retracer la diffusion :** retrouver la première publication et repérer les comptes récents ou coordonnés.
- **Expliquer :** calculer l'indice de fiabilité, expliquer chaque indice avec des mots simples et rédiger un message clair pour les proches.

Une personne seule mettrait des heures à faire ces vérifications ; l'IA les fait en quelques secondes. **Ce que garde l'humain : la décision d'envoyer ou non, toujours.**

## 7.2. Ce qui est réaliste pendant le pilote

Le prototype du pilote s'appuie sur des outils existants (tableau 7) : un modèle d'IA accessible par API (Mistral AI) pour analyser le contenu et rédiger les explications, l'API gratuite Google Fact Check Tools pour retrouver les vérifications déjà publiées, et une base de 50 rumeurs fréquentes déjà vérifiées. Le pilote vérifie surtout les textes, les liens et les captures d'écran. L'analyse avancée des images et de la diffusion (chemin d'une vidéo, comptes coordonnés), montrée dans la maquette, demande des outils spécialisés et un accès aux données des plateformes : elle fait partie de la version complète, après le pilote.

## 7.3. Un encadrement humain

Nous ne prétendons pas garantir seuls la fiabilité de l'outil. Pendant le pilote, un enseignant en journalisme valide les explications de notre base de rumeurs, et chaque contestation est relue par un vérificateur humain. Après le pilote, nous voulons réunir un comité de relecture indépendant (journalistes fact-checkeurs, chercheurs en IA et en sciences sociales, enseignants en éducation aux médias), qui contrôle les résultats et intervient sur les cas complexes.

## 7.4. Une IA indépendante

Un groupe politique ou une entreprise pourrait chercher à influencer nos résultats, par exemple pour faire passer une vraie vidéo pour un deepfake. Vérif'IA deviendrait alors l'outil de manipulation qu'il combat. Nos parades :

- **Pas de label de l'État :** personne n'a le monopole de la vérité, et un outil de vérification doit rester indépendant de tout pouvoir politique. Notre crédibilité repose sur la transparence, pas sur une certification.
- **Une méthode transparente :** chaque résultat cite ses sources et explique ses indices.
- **Des contrôles réguliers :** audits indépendants des résultats.
- **Des techniques, pas des opinions :** l'outil vise les techniques de manipulation (faux comptes, diffusion coordonnée, images détournées), jamais les opinions.

## 7.5. Protéger les utilisateurs

- **Leur vie privée,** et celle des personnes visibles dans les contenus analysés : respect du RGPD, statistiques anonymes, données hébergées en France ; pour les lycéens mineurs, accord des lycées et information des parents.
- **Leur liberté de jugement :** Vérif'IA ne bloque ni ne supprime aucun contenu. Chaque indice est expliqué et peut être contesté. Le badge récompense des habitudes, pas le fait d'avoir « raison ».

> **Notre principe : l'IA analyse, les experts encadrent, l'utilisateur décide.**

# 8. Impact et déploiement

Cette dernière partie présente la manière dont Vérif'IA passe de l'idée au terrain. Elle répond à quatre questions : par quelles étapes le projet sera-t-il déployé ? Comment le ferons-nous connaître ? Avec quels partenaires ? Comment mesurerons-nous son impact ? Notre principe est simple : commencer petit, prouver l'utilité de l'outil, puis grandir.

## 8.1. Étapes

Le déploiement prend la forme d'un pilote de six mois, d'octobre 2026 à mars 2027, découpé en trois phases : préparer, tester, élargir. Nous sommes déjà dans la première phase : la maquette cliquable est prête. Notre équipe (groupe 9) se répartit en quatre pôles (Produit & IA, Contenu & vérification, Partenariats, Communication), qui travaillent en parallèle à chaque phase.

### a. Feuille de route sur six mois (roadmap)

: Tableau 4 – Feuille de route du pilote

| Pôle | Phase 1 – Préparer (oct.–nov. 2026) | Phase 2 – Tester (déc. 2026 – janv. 2027) | Phase 3 – Élargir (févr.–mars 2027) |
|:-----------|:--------------------|:--------------------|:--------------------|
| **Objectif** | Disposer d'un prototype fonctionnel et de 100 testeurs | Vérifier que les testeurs utilisent l'outil et qu'il influence leur décision de partager | Passer à 500 utilisateurs et préparer la suite |
| **Produit & IA** | Maquette cliquable ; prototype v1 développé par l'équipe avec un assistant de code IA ; tests internes | Lancer le pilote ; corriger les bugs chaque semaine | Mettre en ligne une version améliorée (v2) ; assurer la stabilité |
| **Contenu & vérification** | Base de 50 rumeurs fréquentes déjà vérifiées ; explications validées par un enseignant en journalisme | Examiner chaque contestation ; enrichir la base | Créer un kit pour les ateliers en médiathèque et en lycée |
| **Partenariats** | Accord avec 2 lycées, un enseignant en journalisme et le BDE de l'EFAP ; charte de protection des données (RGPD) | 2 ateliers d'éducation aux médias en classe | Étendre à 5 lycées et aux médiathèques (parents, seniors) ; préparer le dossier de financement |
| **Communication** | Identité de marque ; recruter 100 testeurs (lycéens et étudiants de l'EFAP) | Campagne « Vérifie en premier » ; suivi des KPI chaque semaine ; 10 entretiens | Mobiliser des micro-influenceurs et des médias locaux ; publier le bilan du pilote |
| **Conditions de passage** | Prototype fonctionnel et 100 testeurs | Seuils KPI atteints fin janvier | 500 utilisateurs |

### b. Points de contrôle

Chaque phase se termine par un point de contrôle : nous ne passons à la phase suivante que si la condition fixée est remplie (dernière ligne du tableau 4). Fin novembre, le prototype doit fonctionner et 100 testeurs doivent être inscrits. Fin janvier, les seuils de mi-parcours des KPI doivent être atteints (tableau 10) ; sinon, deux semaines sont consacrées aux corrections avant d'élargir. Fin mars, le pilote est validé s'il réunit 500 utilisateurs et atteint ses objectifs. Ces points de contrôle évitent d'élargir un outil qui ne serait pas encore utile.

### c. Et après le pilote ?

Le pilote s'achève à la veille de l'élection présidentielle d'avril 2027, période où la désinformation est la plus intense. Pendant la campagne électorale, Vérif'IA continuera de fonctionner avec ses 500 utilisateurs : ce sera un test en conditions réelles. Si les résultats sont concluants, nous présenterons notre bilan à des médias de fact-checking et à des financeurs plus importants, en vue d'un déploiement national à la rentrée 2027 et d'une ouverture à de nouveaux publics, comme les jeunes actifs.

## 8.2. Campagne de lancement : « Vérifie en premier »

Un outil n'est utile que s'il est connu et utilisé. Notre campagne accompagne les trois phases du pilote avec un double objectif chiffré : recruter 100 testeurs fin novembre 2026, puis atteindre 500 utilisateurs fin mars 2027. Son budget reste modeste (entre 500 et 1 000 euros environ), car elle s'appuie surtout sur notre réseau, sur nos partenaires et sur des contenus produits par l'équipe.

### a. Le concept

La campagne part d'un constat sur notre cible principale : chez les jeunes, partager une information en premier, c'est être dans le coup. Notre campagne retourne ce code : le prestige ne va plus à celui qui partage en premier, mais à celui qui vérifie en premier.

Le ton se veut complice et drôle, jamais moralisateur. Nous ne diffusons jamais une fausse information sans son démenti : chaque défi porte sur une rumeur déjà démentie, et la réponse figure dans le même contenu.

- **Message clé :** « Sois le premier à vérifier, pas le premier à partager. »
- **Signature :** « Vérif'IA – Avant de croire. Avant de partager. Vérifiez. »

### b. Le dispositif en trois temps

: Tableau 5 – Calendrier de la campagne

| Temps | Période | Cible | Objectif | Actions | Canaux |
|:--------|:--------|:----------|:---------|:--------------------|:---------|
| **1. Recruter** | Phase 1 (nov. 2026) | Lycéens des 2 lycées partenaires et étudiants de l'EFAP | 100 testeurs inscrits | Présentation en classe et au BDE ; affiches avec QR code ; vidéo teaser « 10 secondes pour vérifier » | WhatsApp, Instagram de l'EFAP et du BDE, affichage |
| **2. Activer** | Phase 2 (déc. 2026 – janv. 2027) | Les 100 testeurs et leurs amis | Faire utiliser l'outil et lancer le bouche-à-oreille | Défi hebdomadaire #VérifieEnPremier : une rumeur déjà démentie à vérifier le plus vite possible ; 2 ateliers d'éducation aux médias en classe | TikTok, Instagram, ateliers |
| **3. Amplifier** | Phase 3 (févr.–mars 2027) | Nouveaux lycées et parents | Atteindre 500 utilisateurs | 3 à 5 micro-influenceurs ; Semaine de la presse (mars) ; vidéos « Le Groupe Famille » et ateliers en médiathèque pour les parents ; communiqué « Ce que 100 lycéens ont appris en deux mois » | Instagram, TikTok, Facebook, radio campus, presse locale |

### c. Les piliers éditoriaux (content pillars)

Pour rester cohérente pendant six mois, la campagne s'organise autour de quatre piliers éditoriaux. Chacun répond à un objectif précis, du premier contact avec la marque jusqu'à la recommandation.

: Tableau 6 – Piliers éditoriaux de la campagne

| Pilier | Objectif | Contenus types | Formats et canaux | Part |
|:-------------|:----------|:--------------------|:---------------|:----|
| **1. « Le Groupe Famille »** (humour) | Se faire connaître | Mini-fictions sur la vie d'un groupe : le tonton qui transfère tout, l'ado qui vérifie avant tout le monde | Vidéos courtes (30 s) sur TikTok, Instagram Reels et Facebook | 30 % |
| **2. « Les ficelles de la manip' »** (pédagogie) | Repérer les techniques | Une technique décryptée par publication (urgence, faux expert, image recyclée…) ; le défi #VérifieEnPremier | Carrousels Instagram, vidéos courtes, supports d'atelier | 30 % |
| **3. « Vérif'IA, mode d'emploi »** (produit) | Faire essayer | Tutoriel en 30 secondes ; ce que fait l'IA et ce que décide l'utilisateur ; questions fréquentes (gratuité, données) | Stories, vidéos courtes, FAQ | 20 % |
| **4. « La parole aux testeurs »** (preuve sociale) | Convaincre | Témoignages de testeurs, chiffres du pilote, retours des ateliers en lycée et en médiathèque | Publications Instagram, communiqué de presse, contenus des micro-influenceurs | 20 % |

### d. Exemple de contenu : un épisode du défi #VérifieEnPremier

**Format :** vidéo TikTok et Instagram Reels de 20 secondes, publiée chaque semaine en phase 2.

- **Plan 1 (0–3 s)** – Texte à l'écran : « Défi #VérifieEnPremier de la semaine. Tu partagerais ? »
- **Plan 2 (3–8 s)** – Capture d'un message qui circule : « À partir de janvier, WhatsApp devient payant. Partage à tous tes contacts ! »
- **Plan 3 (8–15 s)** – Vérif'IA analyse le message en direct. Résultat : « Probablement faux » : aucune source officielle, ton alarmiste, incitation à partager.
- **Plan 4 (15–20 s)** – Texte final : « Rumeur déjà démentie. Sois le premier à vérifier, pas le premier à partager. » Logo Vérif'IA.
- **Légende :** « En combien de secondes tu l'as vérifiée ? Dis-le en commentaire #VérifieEnPremier »

Le démenti apparaît dans la même vidéo : la rumeur n'est jamais diffusée seule.

## 8.3. Partenaires

### a. Ressources mobilisées sans partenariat

: Tableau 7 – Ressources technologiques et infrastructures

| Ressource | À quoi ça sert |
|:-------------------------------|:-------------------------------|
| Assistant de code IA (ex. Claude) | Développer le prototype nous-mêmes, sans développeur externe |
| Modèle d'IA accessible par API (ex. Mistral AI, acteur français) | Analyser les contenus et rédiger les explications, à faible coût |
| Google Fact Check Tools (API gratuite) | Retrouver les vérifications déjà publiées sur une rumeur |
| Articles publics des fact-checkeurs (AFP Factuel, Les Décodeurs…) | Les citer avec un lien, sans partenariat nécessaire |
| Hébergement en France (ex. OVHcloud) | Stocker les données en France, à faible coût |

### b. Partenaires à notre échelle

: Tableau 8 – Cartographie des partenaires

| Besoin | Partenaire | Ce qu'il apporte | Ce qu'il y gagne | Comment l'approcher | Phase |
|:--------|:------------|:-----------|:-----------|:-----------|:----|
| **Tester** | L'EFAP et son BDE | Les premiers testeurs et des ambassadeurs | Un projet étudiant vitrine | Présentation au BDE, e-mail interne | 1 |
| **Tester** | 2 lycées partenaires (professeurs documentalistes) | Des testeurs lycéens et des ateliers en classe | Un support pédagogique gratuit | Rendez-vous avec le proviseur et le professeur documentaliste | 1 et 2 |
| **Vérifier** | Un enseignant en journalisme | La validation des explications et l'examen des contestations | Un cas pratique réel pour ses étudiants | E-mail au responsable pédagogique | 1 et 2 |
| **Atteindre les familles** | Médiathèques municipales, associations de parents d'élèves | Des ateliers numériques avec des parents et des seniors | Un contenu concret pour leurs ateliers | Rendez-vous avec le responsable numérique | 3 |
| **Faire connaître** | Micro-influenceurs (10 000 à 50 000 abonnés) | Une visibilité auprès des jeunes | Un contenu utile et valorisant | Message privé avec une idée de contenu | 3 |
| **Faire connaître** | Médias locaux et étudiants (radio campus, presse locale) | Une couverture médiatique | Une belle histoire locale | Communiqué de presse | 3 |
| **Financer la suite** | PEPITE (statut d'étudiant-entrepreneur), financement participatif (Ulule), prix étudiants | Le financement de l'après-pilote | Des projets étudiants à impact, au cœur de leur mission | Candidature | 3 |

### c. Risques et parades

: Tableau 9 – Cartographie des risques et solutions

| Risques | Parades |
|:----------------------|:----------------------------------------|
| Les partenaires ne répondent pas | Commencer par notre réseau : l'EFAP et son BDE, dont les étudiants peuvent tester si un lycée tarde |
| Une explication est fausse ou imprécise | Explications validées par un enseignant en journalisme ; chaque contestation est examinée ; en cas de doute, l'outil affiche « Douteux » et explique pourquoi, sans jamais décider à la place de l'utilisateur |
| Le budget manque | Outils gratuits ou peu coûteux et pilote volontairement petit (100 puis 500 utilisateurs) : coût total inférieur à 2 000 €, autofinancé par l'équipe ou couvert par un prix étudiant |
| Testeurs mineurs et données personnelles | Accord des lycées et information des parents ; statistiques anonymes ; données hébergées en France (charte RGPD) |

## 8.4. Indicateurs clés de performance (KPI)

: Tableau 10 – Indicateurs du pilote

| KPI | Question | Ce qu'on mesure | Méthode | Seuil fin janvier 2027 | Objectif fin mars 2027 |
|:---------|:----------|:---------------|:---------------|:------|:------|
| **Réflexe** | Les utilisateurs reviennent-ils ? | % de testeurs qui font au moins 2 vérifications par mois | Statistiques anonymes de l'assistant | ≥ 30 % | ≥ 40 % |
| **Partages évités** | L'outil change-t-il la décision ? | % des résultats « Douteux » ou « Probablement faux » suivis du choix « je ne partage pas » | Choix enregistré après chaque résultat, complété par 10 entretiens | ≥ 40 % | ≥ 50 % |
| **Clarté** | Comprend-on pourquoi ? | % de testeurs qui jugent l'explication claire (note d'au moins 4/5) | Mini-questionnaire dans l'assistant | ≥ 70 % | ≥ 80 % |

Ces chiffres ne sont pas des prévisions mais des seuils de décision : le seuil de fin janvier conditionne le passage à la phase 3, et l'objectif de fin mars valide le pilote. Fixés de manière prudente pour une première expérimentation, ils seront ajustés à partir des données réelles.

# 9. Notre usage de l'IA pour construire le projet

Nous avons utilisé l'IA à chaque étape, en appliquant le même principe que dans Vérif'IA : l'IA propose, l'équipe vérifie et décide.

- **La maquette :** codée par l'équipe avec un assistant de code IA (Claude), puis mise en ligne.
- **Les visuels :** les portraits des personas ont été générés par IA.
- **La rédaction :** un assistant IA nous a aidés à relire et à structurer nos textes ; les choix de fond (cible, concept, chiffres, partenaires) sont ceux de l'équipe.
- **Dans le produit :** un modèle d'IA (Mistral AI) analyse les contenus et rédige les explications (partie 7).

# L'équipe – Groupe 9

Hiba Gherraby · Shems Mrini · Eugenia Colmenares · Olivia Clerico · Ngoc Nhi Luu
