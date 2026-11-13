# TP 1 : Diagrammes de Cas d’Utilisation `UML` 

Les diagrammes des cas d’utilisation ( _Use Case_ en anglais) permettent aux informaticiens d’une part et aux utilisateurs d’autre part, de se mettre d’accord sur les besoins de l’application. Lorsqu’on veut concevoir et réaliser une application (un logiciel), généralement on construit d’abord le diagramme des cas d’utilisation. Ainsi, les objectifs sont : 

- de recueillir, 

- d’analyser, 

- d’organiser les besoins, et 

- de recenser les grandes fonctionnalités d’un système. 

Ces informations doivent être déduites à travers le cahier des charges établi par le client (généralement, l’informaticien l’assiste afin de préciser ce dernier). Ainsi le diagramme de cas d’utilisation peut évoluer au fur et à mesure que les discussions avancent. Dans tous les cas, il est interdit de prendre l’initiative et d’ajouter des fonctionnalités au système **sans consultation préalable** avec le client. Tout ajout de fonctionnalité doit être approuvé par le client ou ressortir de l’éoncé. 

## **1 Acteurs** 

Un acteur représente un rôle joué par une entité externe (utilisateur humain, dispositif matériel ou autre système) qui **interagit directement avec le système étudié** . Un acteur peut consulter et/ou modifier directement l’état du système, en émettant et/ou en recevant des messages susceptibles d’être porteurs de données. 

D’après Audibert (voir réf. dans CM), 

Une manière de faciliter la recherche des acteurs est d’ **imaginer les frontières du système** . Tout ce qui est à l’extérieur et qui interagit avec le système est un acteur, tout ce qui est à l’intérieur est une fonctionnalité à modéliser. 

En `UML` on représente les acteurs par un pictogramme humano¨ıde ( _stick man_ en anglais), avec le nom de l’acteur sous le dessin. Si l’acteur n’est pas un humain, on peut le représenter sous forme d’un classeur rectangulaire stéréotypé `<<actor>>` . Un exemple est donné dans la figure ci-dessous. 



<!-- Start of picture text -->
mot-clé<br><<actor>>SI banque a<br>stick man Client<br><!-- End of picture text -->

Figure 1: Représentations graphiques d’un acteur 

## **2 Cas d’utilisation** 

Un cas d’utilisation représente un ensemble de séquences d’actions qui sont réalisées par le système et qui produisent un résultat observable ” _intéressant_ ” pour un acteur (voire plusieurs acteurs). Chaque cas d’utilisation correspond donc à une fonction métier du système, selon le point de vue d’un de ses acteurs. Par conséquent, on nomme les cas d’utilisation par un verbe à l’infinitif suivi d’un complément. 

L’ensemble des cas d’utilisation doit décrire exhaustivement les exigences fonctionnelles du système, tout en gardant un niveau suffisant d’abstraction. 

Les liens de dépendance et généralisation entre les cas d’utilisation permettront une meilleure décomposition de votre diagramme. 

Une fois les cas d’utilisation identifiés, il faut les décrire à travers des scenarios ( **description textuelle** ). 

### **2.1 à propos des diagrammes de cas d’utilisation** 

D’après Audibert (2014). 

#### **2.1.1 Relations dans les cas d’utilisation** 

Il est important de noter qu’une utilisation poussée des relations n’est pas primordiale dans la rédaction des cas d’utilisation et donc dans l’expression du besoin. Ces relations peuvent être utiles dans certains cas, mais une trop forte focalisation sur leur usage conduit souvent à une perte de temps ou à un usage faussé, pour une valeur ajoutée, au final, relativement faible. **L’effort doit essentiellement se porter sur l’identification des acteurs, des cas d’utilisation et des associations simples entre acteurs et cas d’utilisation.** 

#### **2.1.2 Diagramme de cas d’utilisation** 

Les diagrammes de cas sont unanimement reconnus comme cantonnés à l’ingénierie des besoins, et ne peuvent être qualifiés de modélisation à proprement parler. D’ailleurs, de nombreux éléments desscriptifs sont en langage naturel. De plus, **ils ne correspondent pas stricto sensus à une approche objet** . En effet, capturer les besoins, les découvrir, les réfuter, les consolider, . . . , correspond plus à une analyse fonctionnelle classique. 

## **Consignes** 

- Durant le TD, vous travaillerez d’abord sur papier. 

- Ensuite, vous réaliserez vos diagrammes sur le logiciel `Star UML` . Le logiciel permet notamment d’exporter vos diagrammes en format `.pdf` . 

- Vous pourrez également le déposer sur git. 

## **Exercice 1 – Réservation de trains** 

Proposez un diagramme de cas d’utilisation pour un distributeur de billets de train. Le distributeur permet aux voyageurs l’achat des billets aller simple, des abonnements hebdomadaires ou mensuels. Une entité externe au portail de réservation (la machine centrale) mets à jour régulièrement les tarifs des billets. Pensez à inclure les options d’erreur : temps trop long durant la réservation, annulation de la transaction ou encore plus de papier dans la machine. 

## **Exercice 2 – contrôle d’un ascenseur** 

1. Construisez le diagramme de cas d’utilisation pour le système de contrôle simplifié d’un ascenseur respectant les contraintes fonctionnelles suivantes : 

   - L’utilisateur (passager) doit pouvoir appeler un ascenseur et choisir l’étage de destination. 

   - Lorsque l’utilisateur appuie sur le bouton extérieur pour appeler l’ascenseur ou sur le bouton intérieur pour choisir l’étage, le système affiche sur un panneau d’affichage un message. 

   - Lorsque l’utilisateur appuie sur un bouton le système de contrôle ferme/ouvre la porte. 

   - Lorsque l’utilisateur appuie sur un bouton le système actionne le déplacement de l’ascenseur vers la destination correspondante. 

   - Lorsque l’utilisateur quitte l’ascenseur, le panneau d’affichage s’éteint. 

2. Donnez la description textuelle du cas d’utilisation ” _Choisir étage_ ” 

## **Exercice 3 – Portail livraison repas** 

Vous êtes chargé de modéliser le fonctionnement d’un portail internet qui, dans le cadre des services aux personnes, gère la livraison à domicile de plateaux repas dont la préparation proprement dite est sous-traitée à une cuisine industrielle. Vous devez prendre en compte : 

   - Les inscriptions individuelles et les inscriptions par groupe (maisons de retraite par exemple) 

   - Les inscriptions subventionnées ou non (par la sécurité sociale, par un groupe d’assurance, etc.) 

   - Le choix des menus par internet ou par e-mail (réservé aux groupes) 

   - La vérification des menus par rapport aux éventuels régimes alimentaires (qui sont connus du service de livraison des repas) 

   - Le lancement de l’ordre de commande aux cuisines, les livraisons et les facturations 

1. A<sup>`</sup> partir du texte proposé, identifiez les acteurs. 

2. Toujours à partir du texte proposé (sans ajouter des informations supplémentaires), proposez un diagramme de cas d’utilisation. 

## **Exercice 4 – Etude**<sup>**´**</sup> **d’un Guichet Automatique de Banque** 

_Sujet adapté d’une étude de cas présentée dans le livre ”UML par la pratique” de Pascal Roques, édition Eyrolles, 2009._ 

On souhaite établir le cahier des charges pour la réalisation d’un système simplifié de Guichet Automatique de Banque (GAB) de la banque `MaB’Arnaque` . Le GAB offre les services suivants: 

   - Distribution d’argent à tout Porteur de carte de crédit via un lecteur de carte et un distributeur de billets (y compris pour les non-clients de `MaB’Arnaque` ) 

   - Consultation de solde de compte, dépôt en numéraire et dépôt de chèques pour les clients porteurs d’une carte de crédit de la banque adossée au GAB ( `MaB’Arnaque` ). 

   - Les transactions sont sécurisées quel que soit le type de carte de crédit insérée. 

   - Il est parfois nécessaire de recharger le distributeur. 

1. Identifiez les acteurs qui interagissent avec le GAB. 

2. Identifier les cas d’utilisation du système. 

3. Trouvez les acteurs secondaires. 

4. Construisez un diagramme de cas d’utilisation 

5. Pour chaque cas d’utilisation, établissez la liste des scénarios possibles et proposez une description textuelle du cas d’utilisation. 

