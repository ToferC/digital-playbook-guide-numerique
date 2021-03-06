---
layout: default
title: Outil décisionnel du nuage approprié (ébauche)
lang: fr
altLang: en
altLangPage: cloud-decision-tool
collectionDirectory: views-vues/cloud-nuage
questions:
  "1": Délicatesse
  "1-a1": Les intervenants n’ont pas soulevé des préoccupations concernant la délicatesse des données.
  "1-a2": Les intervenants perçoivent que la délicatesse des données est élevée.
  "2": Financier
  "2-a1": Le budget est disponible pour appuyer l’adoption d’un modèle de dépenses opérationnelles; les coûts augmenteront et chuteront avec la consommation des ressources.
  "2-a2": Le budget est disponible pour appuyer l’adoption d’un modèle de dépenses en capital; la capacité à prévoir des investissements périodiques dans une infrastructure et en innovation en évolution constante.
  "3": Legs
  "3-a1": L’application peut fonctionner dans un environnement en nuage et le matériel virtualisé ou spécialisé requis est offert dans le cadre d’un environnement en nuage.
  "3-a2": L’application doit fonctionner dans un environnement hors-nuage et il faut du matériel très spécialisé.
  "4": Commercialisé
  "4-a1": L’application peut fonctionner dans le cadre des offres normalisées et des ANS relatives au nuage public.
  "4-a2": L’application exige la personnalisation des offres et des ANS.
  "5": Endroit
  "5-a1": L’application n’est pas susceptible aux problèmes de latence qui peuvent survenir en raison de l’achalandage qui passe par un circuit supplémentaire.
  "5-a2": L’application est susceptible aux problèmes de latence qui peuvent survenir en raison de l’achalandage qui passe par un circuit supplémentaire.
  "6": Connectivité
  "6-a1": L’application n’a pas de transaction volumineuse avec une base de données ou une application sur les lieux.
  "6-a2": L’application a des transactions volumineuses avec une base de données ou une application sur les lieux.
  "7": Rapidité
  "7-a1": On désire avoir un accès rapide aux services. Est-ce que les services requis sont accessibles sur demande?
  "7-a2": Peut tolérer le temps nécessaire afin de procéder à la mise en œuvre des services qui peuvent, à l’heure actuelle, ne pas être accessibles sur demande.
  "8": Longévité
  "8-sub": L’application est censée répondre à
  "8-a1": un besoin à court terme
  "8-a2": un besoin à long terme
  "9": Elasticité
  "9-sub": Avec le temps, les exigences en matière de ressources de l’application
  "9-a1": demeureront stables
  "9-a2": croîtront et/ou diminueront
  "10": Innovation
  "10-a1": On voudra que le projet tire profit des nouvelles tendances technologiques au fur et à mesure qu’elles sont mises en vente sur le marché.
  "10-a2": On ne souhaite pas que l’application tire profit des nouvelles tendances technologiques, et celle-ci demeurera stable.
  "10-a3": Aucune nouvelle technologie n’est requise.
  "11": Dév. opérations
  "11-a1": Désire un accès rapide à un ensemble d’outils pour appuyer le développement d’applications comme plateforme de services sans faire un investissement en capital.
  "11-a2": Est prêt investir pour déployer des outils de développement d’applications pour appuyer le projet.
public: Public
private: Privé
nonCloud: Hors-nuage
mandatorySection: Obligatoire
highlyRatedSection: "Bien coté [20 points chacun]"
ratedSection: "Coté [10 points chacun]"
mandatoryMet: Obligatoire respecté
ratedTotals: Totaux cotés
cloudTypes:
 - "public-cloud"
 - "private-cloud"
 - "non-cloud"
criteriaTags:
 - "sensitivity"
 - "financial"
 - "legacy"
 - "commoditized"
 - "location"
 - "connectivity"
 - "speed"
 - "longevity"
 - "elasticity"
 - "innovation"
 - "devops"
---
{% assign dataVariable = site.playbookData[page.lang] %}{%
assign dataSource = site.data[dataVariable] %}
<div class="wb-inview" data-inview="progress-overlay">

Il vous est possible d’utiliser le modèle suivant afin de vous aider à décider du bon modèle de déploiement du nuage approprié pour votre contexte opérationnel.

</div>

{% include views-vues/cloud-nuage/cloud-decision-tool-outil-nuage-decisionnel-questionnaire.html %}

{% include views-vues/cloud-nuage/cloud-decision-tool-outil-nuage-decisionnel-resultats.html %}
