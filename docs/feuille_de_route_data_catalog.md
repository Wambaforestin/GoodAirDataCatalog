# Feuille de Route : Implémentation du Data Catalog GoodAir

Ce document retrace les grandes étapes à suivre pour mener à bien la mise en place du Data Catalog pour le laboratoire TotalGreen, en respectant une séparation stricte entre la conception fonctionnelle et l'implémentation technique.

## PHASE 1 : Conception du Métamodèle (Focus Actuel)

*Objectif : Définir la structure théorique, les concepts et les règles du catalogue sans écrire une ligne de code.*

1. **Business Requirements et Use Cases**
   * Affiner les cas d'usage précis (ex: "Un chercheur veut trouver les données d'historique des canicules").

2. **Définition des Domaines de Données (Data Domains)**
   * Structurer les domaines autour des capacités du laboratoire (ex: Qualité de l'Air, Météorologie).

3. **Définition des Actifs (Data Assets et Data Products)**
   * Identifier ce qui sera catalogué (Vues SQL, Dashboards Metabase, Modèles ML, Table SQL) pour masquer la complexité technique de l'entrepôt.

4. **Glossaire Métier (Business Glossary)**
   * Définir la structure sémantique (Termes, Définitions, Acronymes comme AQI, PM2.5).

5. **Gouvernance et Rôles (Roles et Responsibilities)**
   * Définir qui fait quoi (Data Owner, Data Steward, Data Engineer, Consommateur).

6. **Conception du Métamodèle (Metamodel Design)**

   * Schéma du métamodèle : Concevoir la structure globale (entités et attributs de notre catalogue).
   * Relations : Établir les liens entre les concepts (ce qui inclut naturellement la traçabilité et le lignage).
   * Outil de modélisation : Implémenter le schéma visuellement avec un outil de modélisation (diagramme entité-relation).

## PHASE 2 : Implémentation Technique (À venir)

*Objectif : Concevoir et developper l'application web du catalogue.*

1. **Conception UI/UX (Maquettes)**
   * Design des différentes pages de l'application.
   * Design des parcours de connexion et des profils utilisateurs.

2. **Choix de l'Architecture Technique**
   * Validation de l'architecture technique (Backend, Frontend, API).
   * Validation de la base de données (PostgreSQL existant ou base dédiée).
   * Identification des technologies appropriées.
  
3. **Les fonctionnalités du catalogue**
   * Moteur de recherche simple.
   * Authentification des utilisateurs (Login).
   Note : D'autres fonctionnalités sont toujours en cours de décision.
   * **Nouveau :** Authentification des utilisateurs (Login).
   * **Nouveau :** Identification des patterns d'utilisation (historique de recherche, habitudes et requêtes fréquentes par utilisateur).

4. **Développement de l'Application Web**
   * Backend, API, et Frontend.

5. **Conteneurisation et Déploiement**
   * Création de l'image Docker de l'application et mise en réseau.

## PHASE 3 : Opérationnalisation (À venir)

*Objectif : Faire vivre le catalogue et mesurer son adoption.*

1. **Processus de publication**
   * Workflow pour ajouter un nouveau Data Product au catalogue.

2. **Mise en place des KPIs**
   * Mesurer l'utilisation du catalogue par les chercheurs de TotalGreen.

---

## Ressources et Références utiles

*Ces liens servent de base de réflexion pour affiner les concepts clés du catalogue au fil de l'avancement du projet :*

* [What is a Data Product? (Coalesce)](https://coalesce.io/data-insights/what-is-a-data-product/)
* [How Data Catalogs Help With Data Quality (Actian)](https://www.actian.com/blog/data-quality/how-data-catalogs-help-with-data-quality/)
* [Collibra Data Dictionary Insights (Murdio)](https://murdio.com/insights/collibra-data-dictionary/)
