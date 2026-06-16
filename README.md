<div align="center">

# Zabbix Map Builder

### Design clear, professional Zabbix network maps in minutes, then publish them straight to Zabbix.

[![Latest release](https://img.shields.io/github/v/release/bboqueho/map-builder-releases?label=latest&color=0a6240)](https://github.com/bboqueho/map-builder-releases/releases/latest)
![Platform](https://img.shields.io/badge/platform-Windows%2010%2F11-blue)
![Made by Orsenna](https://img.shields.io/badge/by-Orsenna-0a6240)

[**⬇ Download**](https://github.com/bboqueho/map-builder-releases/releases/latest) · [Features](#features) · [Quick start](#quick-start) · [Licensing](#licensing) · [Français 🇫🇷](#français)

</div>

---

## What is Zabbix Map Builder?

**Zabbix Map Builder** is a desktop application that turns your Zabbix inventory into clean, readable network maps, without the frustration of the built-in map editor.

Connect it to your Zabbix server, pick the hosts you care about, arrange them on a canvas (or let the app lay them out for you), style the links, and **publish the result back to Zabbix as a native map** in one click. Your NOC sees a polished topology; you keep full control.

Everything runs **locally on your machine**. The only system the application talks to is *your* Zabbix server: no cloud, no account, no data leaving your network.

**Who it's for:** managed service providers, NOC and monitoring teams, and IT departments that run Zabbix and want presentation-quality maps for dashboards, hand-off documents and client reports.

---

## Features

**Build maps fast**
- Connect to any Zabbix server with a URL and an API token. Multiple servers are supported.
- Import hosts and host groups; automatic layout and topology discovery from your Zabbix data.
- Guided **Wizard** for a map in five steps, or **Expert** mode for full manual control.
- **Link-discovery template**: on first use, the app can create a Zabbix template that collects LLDP/CDP neighbours over SNMP (standard LLDP-MIB + CISCO-CDP-MIB), so topology links are discovered automatically.

**A real editor**
- Drag-and-drop nodes, multi-select (rubber-band and Ctrl/Shift-click), undo/redo, snap-to-grid.
- Link styles to match Zabbix: straight, curved or right-angle, with solid / bold / dotted / dashed lines.
- Group hosts into labelled rectangles, add a large library of network and vendor icons.
- Live link labels: interface, nominal speed and **bandwidth utilisation %**, operational-status colours.

**Publish & share**
- **One-click publish to Zabbix**: your map becomes a real Zabbix map (elements, links, group rectangles).
- Export to **PNG, SVG and PDF** (a multi-page report with cover page, host inventory and link tables).
- Export raw **JSON**, or round-trip through **draw.io / diagrams.net**.

**Built for the real world**
- Native Windows desktop app, fully offline, light on resources.
- French and English interface, switchable at any time.
- Automatic, signed update checks: install new versions in one click.

---

## Quick start

1. **Download** the latest `ZabbixMapBuilder-windows.zip` from the [Releases page](https://github.com/bboqueho/map-builder-releases/releases/latest).
2. **Unzip** it anywhere (for example `C:\Apps\ZabbixMapBuilder`) and run **`ZabbixMapBuilder.exe`**.
3. Follow the **Wizard**:
   1. **Connect**: enter your Zabbix URL (for example `https://zabbix.example.com`) and an **API token**.
   2. **Hosts**: choose the hosts and host groups to place on the map.
   3. **Topology**: let the app draw the links, or add and edit them yourself. On first run, the app offers to install a **link-discovery template** (LLDP/CDP over SNMP) in your Zabbix; assign it to the devices you want to map.
   4. **Style**: set link styles, icons, groups and labels.
   5. **Publish**: push the finished map to Zabbix, or export it as an image or PDF.

> **Getting an API token in Zabbix:** go to *Users → API tokens → Create API token* (Zabbix 6.0 or newer). Assign it to a user that can read the hosts you want to map.

Your map is then live in Zabbix under *Monitoring → Maps*.

---

## Updating

The application checks for new versions on launch. When one is available, a banner appears: click **Install & restart** and the update is downloaded, verified and applied automatically. Your settings, drafts and licence are preserved.

---

## Licensing

Zabbix Map Builder starts with a **free 7-day trial**: full features, no account required.

After the trial, the application needs a **licence file** (`license.key`) issued by Orsenna:

1. Open the application; it displays your **Zabbix ID** (a code like `ZBX-1A2B-3C4D-5E6F`).
2. Send that ID to Orsenna.
3. You receive a `license.key`; place it next to the application and restart.

A licence is tied to your Zabbix instance(s). **One licence can cover several Zabbix servers**: just send all of your Zabbix IDs. Both **perpetual** and **subscription** licences are available.

👉 **Request a licence or a quote:** [orsenna.fr](https://orsenna.fr) · helpdesk@orsenna.fr

---

## System requirements

- **Windows 10 or 11** (64-bit).
- Network access to your Zabbix server (**Zabbix 6.0 or newer** recommended) and an API token.
- For the native window, the **Microsoft WebView2 runtime** (already present on most up-to-date Windows machines; the app falls back to an Edge/Chrome window otherwise).

---

## Support

- 🌐 Website: [orsenna.fr](https://orsenna.fr)
- ✉️ Support: helpdesk@orsenna.fr

This repository hosts the **packaged Windows releases** of Zabbix Map Builder. The source code is private. Each release contains the application (`ZabbixMapBuilder-windows.zip`) and a signed update manifest (`latest.json`) used by the in-app updater.

© Orsenna. *Zabbix™ is a trademark of Zabbix SIA. Zabbix Map Builder is an independent product and is not affiliated with or endorsed by Zabbix SIA.*

<br>

---

<a name="français"></a>
<div align="center">

# Zabbix Map Builder 🇫🇷

### Concevez des cartes réseau Zabbix claires et professionnelles en quelques minutes, puis publiez-les directement dans Zabbix.

[**⬇ Télécharger**](https://github.com/bboqueho/map-builder-releases/releases/latest) · [Fonctionnalités](#fonctionnalités) · [Démarrage rapide](#démarrage-rapide) · [Licence](#licence-1)

</div>

## Qu'est-ce que Zabbix Map Builder ?

**Zabbix Map Builder** est une application de bureau qui transforme votre inventaire Zabbix en cartes réseau lisibles et soignées, sans la frustration de l'éditeur de cartes intégré.

Connectez-la à votre serveur Zabbix, sélectionnez les hosts utiles, disposez-les sur un canevas (ou laissez l'application le faire), mettez en forme les liens, puis **publiez le résultat dans Zabbix sous forme de carte native**, en un clic. Votre NOC voit une topologie propre ; vous gardez la maîtrise totale.

Tout fonctionne **en local sur votre poste**. Le seul système contacté est *votre* serveur Zabbix : aucun cloud, aucun compte, aucune donnée ne sort de votre réseau.

**Pour qui :** infogéreurs (MSP), équipes NOC et supervision, et DSI qui exploitent Zabbix et veulent des cartes de qualité présentation pour leurs tableaux de bord, leurs livrables et leurs rapports clients.

## Fonctionnalités

**Créez vite**
- Connexion à n'importe quel serveur Zabbix via une URL et un jeton API. Plusieurs serveurs possibles.
- Import des hosts et groupes de hosts ; mise en page automatique et découverte de topologie à partir de vos données Zabbix.
- **Assistant** guidé pour une carte en cinq étapes, ou mode **Expert** pour un contrôle manuel complet.
- **Template de découverte des liens** : au premier usage, l'application peut créer un template Zabbix qui collecte le voisinage LLDP/CDP en SNMP (OID standards LLDP-MIB + CISCO-CDP-MIB), pour découvrir automatiquement les liens de topologie.

**Un véritable éditeur**
- Glisser-déposer des nœuds, sélection multiple (rectangle élastique, Ctrl/Maj-clic), annuler/rétablir, aimantation à la grille.
- Styles de liens fidèles à Zabbix : droit, courbe ou orthogonal, en trait plein / gras / pointillé / tireté.
- Regroupement des hosts en rectangles étiquetés, large bibliothèque d'icônes réseau et éditeurs.
- Étiquettes de liens dynamiques : interface, débit nominal et **taux d'utilisation %**, couleurs d'état opérationnel.

**Publiez et partagez**
- **Publication Zabbix en un clic** : votre carte devient une vraie carte Zabbix (éléments, liens, rectangles de groupes).
- Export en **PNG, SVG et PDF** (rapport multi-pages : page de garde, inventaire des hosts, tableaux des liens).
- Export **JSON** brut, ou aller-retour via **draw.io / diagrams.net**.

**Pensé pour le terrain**
- Application de bureau Windows native, entièrement hors-ligne, légère.
- Interface française et anglaise, commutable à tout moment.
- Vérification de mise à jour automatique et signée : installation en un clic.

## Démarrage rapide

1. **Téléchargez** le dernier `ZabbixMapBuilder-windows.zip` depuis la [page Releases](https://github.com/bboqueho/map-builder-releases/releases/latest).
2. **Décompressez-le** où vous voulez (par exemple `C:\Apps\ZabbixMapBuilder`) et lancez **`ZabbixMapBuilder.exe`**.
3. Suivez l'**Assistant** :
   1. **Connexion** : saisissez l'URL Zabbix (par exemple `https://zabbix.exemple.fr`) et un **jeton API**.
   2. **Hosts** : choisissez les hosts et groupes à placer sur la carte.
   3. **Topologie** : laissez l'application tracer les liens, ou ajoutez-les et modifiez-les. Au premier lancement, l'application propose d'installer un **template de découverte des liens** (LLDP/CDP en SNMP) dans votre Zabbix ; assignez-le aux équipements à cartographier.
   4. **Style** : réglez styles de liens, icônes, groupes et étiquettes.
   5. **Publier** : envoyez la carte vers Zabbix, ou exportez-la en image ou PDF.

> **Créer un jeton API dans Zabbix :** allez dans *Utilisateurs → Jetons API → Créer un jeton* (Zabbix 6.0 ou plus récent). Affectez-le à un utilisateur autorisé à lire les hosts à cartographier.

Votre carte est alors dans Zabbix sous *Supervision → Cartes*.

## Mise à jour

L'application vérifie les nouvelles versions au démarrage. Lorsqu'une mise à jour est disponible, une bannière apparaît : cliquez sur **Installer et redémarrer**, elle est téléchargée, vérifiée et appliquée automatiquement. Vos réglages, brouillons et licence sont conservés.

## Licence

Zabbix Map Builder démarre avec un **essai gratuit de 7 jours** : toutes les fonctions, sans compte.

Après l'essai, l'application nécessite un **fichier de licence** (`license.key`) délivré par Orsenna :

1. Ouvrez l'application ; elle affiche votre **ID Zabbix** (un code du type `ZBX-1A2B-3C4D-5E6F`).
2. Envoyez cet ID à Orsenna.
3. Vous recevez un `license.key` ; placez-le à côté de l'application et relancez.

Une licence est liée à votre/vos instance(s) Zabbix. **Une seule licence peut couvrir plusieurs serveurs Zabbix** : il suffit d'envoyer tous vos ID Zabbix. Licences **perpétuelle** et **par abonnement** disponibles.

👉 **Demander une licence ou un devis :** [orsenna.fr](https://orsenna.fr) · helpdesk@orsenna.fr

## Configuration requise

- **Windows 10 ou 11** (64 bits).
- Accès réseau à votre serveur Zabbix (**Zabbix 6.0 ou plus récent** recommandé) et un jeton API.
- Pour la fenêtre native, le **runtime Microsoft WebView2** (déjà présent sur la plupart des Windows à jour ; sinon l'application bascule sur une fenêtre Edge/Chrome).

## Support

- 🌐 Site : [orsenna.fr](https://orsenna.fr)
- ✉️ Support : helpdesk@orsenna.fr

Ce dépôt héberge les **versions Windows packagées** de Zabbix Map Builder. Le code source est privé. Chaque release contient l'application (`ZabbixMapBuilder-windows.zip`) et un manifeste de mise à jour signé (`latest.json`) utilisé par la mise à jour intégrée.

© Orsenna. *Zabbix™ est une marque de Zabbix SIA. Zabbix Map Builder est un produit indépendant, sans affiliation ni approbation de Zabbix SIA.*
