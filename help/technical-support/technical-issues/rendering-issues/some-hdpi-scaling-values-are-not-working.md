---
helpx_url: "https://helpx.adobe.com/fr/substance-3d-painter/technical-support/technical-issues/rendering-issues/some-hdpi-scaling-values-are-not-working.html"
breadcrumb-title: ''
description: Découvrez comment résoudre les problèmes de mise à l’échelle HDPI dans Substance 3D Painter pour une prise en charge appropriée de l’affichage haute résolution.
helpx_creative_field: ""
helpx_description: Painter > Technical support > Technical Issues > Rendering Issues > Some HDPI scaling values are not working
helpx_experience_level: ""
helpx_learn_topic: ""
helpx_tags: ""
title: Certaines valeurs de mise à l’échelle HDPI ne fonctionnent pas
user-guide-description: ''
user-guide-title: ''
source-git-commit: 9f20406f682e0e6a2e9a423e81c5ecfc7430ecfd
workflow-type: tm+mt
source-wordcount: '127'
ht-degree: 0%

---


# Certaines valeurs de mise à l’échelle HDPI ne fonctionnent pas

Sous Windows, certaines valeurs de mise à l’échelle HDPI (utilisées pour mettre à l’échelle l’interface sur les moniteurs haute résolution) peuvent ne pas fonctionner correctement.\
En effet, notre cadre de fenêtres (Qt) ne les prend pas en charge. Nous sommes incapables de le corriger tant qu&#39;il n&#39;est pas géré par les fournisseurs du cadre lui-même.

Voici donc le comportement que vous pouvez rencontrer en fonction de vos paramètres :

* 120 PPP (mise à l&#39;échelle **125 %**) : rendu en 96 PPP (mise à l&#39;échelle **100 %**)
* 144 PPP (**150 %** de mise à l&#39;échelle) : rendu en 192 PPP (**200 %** de mise à l&#39;échelle)
* 168 PPP (mise à l&#39;échelle **175 %**) : rendu en 192 PPP (mise à l&#39;échelle **200 %**)

Pour plus d&#39;informations, voir : <https://bugreports.qt.io/browse/QTBUG-55654>
