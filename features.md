---
layout: default
title: Fonctionnalités — Ifenia
---

<!-- ═══ PAGE HERO ═══ -->
<div class="page-hero">
  <p class="eyebrow">Tout en détail</p>
  <h1>Fonctionnalités <em style="font-style:italic; color:var(--gold);">complètes</em></h1>
  <p>Chaque fonctionnalité d'Ifenia a été pensée pour sublimer l'expérience voyage.</p>
</div>

<!-- ═══ CONTENU ═══ -->
<section class="section section--navy">
  <div class="section-inner">

    <!-- Gestion des voyages -->
    <div class="feature-section reveal">
      <div class="feature-section-header">
        <span class="ico">✈️</span>
        <h2>Gestion des voyages</h2>
      </div>
      <ul class="feature-list">
        <li>Création avec autocomplétion Google Places (destination)</li>
        <li>Catégorie, dates de début et de fin, budget, devise</li>
        <li>Image de couverture personnalisée</li>
        <li>Suggestions d'activités Google Places → ajout automatique</li>
        <li>3 listes pré-créées : Indispensables · À faire avant de partir · À visiter</li>
        <li>Édition complète de tous les champs, suppression du voyage</li>
        <li>Badge statut : Personnel / Partagé / Collaborateur</li>
        <li>Séparation voyages actifs / archivés (date passée)</li>
        <li>Invitation par QR code ou code textuel 8 caractères</li>
        <li>Rejoindre un voyage via code depuis l'écran principal</li>
      </ul>
    </div>

    <!-- 7 Onglets -->
    <div class="feature-section reveal">
      <div class="feature-section-header">
        <span class="ico">📋</span>
        <h2>7 Onglets par voyage</h2>
      </div>

      <div class="tab-grid">
        <div class="tab-card">
          <span class="ico">✅</span>
          <span>Listes</span>
        </div>
        <div class="tab-card">
          <span class="ico">🗺️</span>
          <span>Roadbook</span>
        </div>
        <div class="tab-card">
          <span class="ico">⛅</span>
          <span>Météo</span>
        </div>
        <div class="tab-card">
          <span class="ico">💬</span>
          <span>Messages</span>
        </div>
        <div class="tab-card">
          <span class="ico">💳</span>
          <span>Dépenses</span>
        </div>
        <div class="tab-card">
          <span class="ico">📸</span>
          <span>Photos</span>
        </div>
        <div class="tab-card">
          <span class="ico">🗳️</span>
          <span>Votes</span>
        </div>
      </div>

      <ul class="feature-list">
        <li><strong>Listes</strong> — Checklists personnalisées, items avec titre, coché, budget, date</li>
        <li><strong>Roadbook</strong> — Itinéraire unifié trié par jour/heure, créneaux typés</li>
        <li><strong>Météo</strong> — Open-Meteo, quotidien, emoji WMO, 16 jours à l'avance</li>
        <li><strong>Messages</strong> — Chat temps réel entre collaborateurs via Firestore</li>
        <li><strong>Dépenses</strong> — Partagées, répartition configurable, soldes automatiques</li>
        <li><strong>Photos</strong> — Album collaboratif, grille 3 colonnes, upload compressé</li>
        <li><strong>Votes</strong> — Sondages temps réel, 2–4 options, barres de progression live</li>
      </ul>
    </div>

    <!-- Carte Google Maps -->
    <div class="feature-section reveal">
      <div class="feature-section-header">
        <span class="ico">📍</span>
        <h2>Carte interactive</h2>
      </div>
      <ul class="feature-list">
        <li>Vue plein écran depuis le Roadbook</li>
        <li>Marqueur principal sur la destination du voyage</li>
        <li>Marqueurs colorés par type de créneau (visite, restaurant, hôtel, transport, activité)</li>
        <li>Géocodage automatique via Google Geocoding API</li>
        <li>InfoWindow au tap : titre + description du créneau</li>
      </ul>
    </div>

    <!-- Collaboration -->
    <div class="feature-section reveal">
      <div class="feature-section-header">
        <span class="ico">👥</span>
        <h2>Collaboration</h2>
      </div>
      <ul class="feature-list">
        <li>Ajout de collaborateurs par email avec autocomplétion (8 résultats)</li>
        <li>Rôles distincts : owner et editor</li>
        <li>Suppression de collaborateur par le propriétaire</li>
        <li>Invitation par QR code généré ou code 8 caractères</li>
        <li>Notification automatique lors d'une modification de liste</li>
        <li>Badge temps réel Notifications (non-lues)</li>
      </ul>
    </div>

    <!-- Notifications push -->
    <div class="feature-section reveal">
      <div class="feature-section-header">
        <span class="ico">🔔</span>
        <h2>Notifications push (FCM)</h2>
      </div>
      <ul class="feature-list">
        <li>Token FCM stocké dans Firestore users/{uid}.fcmToken</li>
        <li>Notifications foreground via flutter_local_notifications</li>
        <li>Navigation au tap vers le voyage concerné</li>
        <li>Cloud Function déclenchée à la création d'une notification</li>
        <li>4 préférences granulaires : activité collaborateurs, invitations, rappels, changements majeurs</li>
      </ul>
    </div>

    <!-- Export PDF -->
    <div class="feature-section reveal">
      <div class="feature-section-header">
        <span class="ico">📄</span>
        <h2>Export PDF</h2>
      </div>
      <ul class="feature-list">
        <li>Page de couverture avec image du voyage</li>
        <li>Informations générales et liste des collaborateurs</li>
        <li>Itinéraire jour par jour (Roadbook)</li>
        <li>Checklists complètes (items cochés et non cochés)</li>
        <li>Récapitulatif des dépenses et soldes par personne</li>
        <li>Partage natif via impression ou envoi (share_plus)</li>
      </ul>
    </div>

    <!-- Exploration -->
    <div class="feature-section reveal">
      <div class="feature-section-header">
        <span class="ico">🔍</span>
        <h2>Exploration (Search)</h2>
      </div>
      <ul class="feature-list">
        <li>3 onglets : Lieux &amp; Attractions · Hôtels · Restaurants</li>
        <li>Recherche via Google Places API (top 10 résultats)</li>
        <li>Affichage : photo, nom, adresse, rating, type de cuisine</li>
        <li>Navigation vers Google Maps depuis les résultats</li>
      </ul>
    </div>

    <!-- Communauté -->
    <div class="feature-section reveal">
      <div class="feature-section-header">
        <span class="ico">🌍</span>
        <h2>Listes communautaires</h2>
      </div>
      <ul class="feature-list">
        <li>Partager une liste d'un voyage vers la communauté</li>
        <li>Découvrir : récentes / populaires / favoris</li>
        <li>Like / Unlike en temps réel</li>
        <li>Signaler une liste inappropriée</li>
        <li>Importer une liste communautaire dans un voyage</li>
      </ul>
    </div>

    <!-- Paramètres -->
    <div class="feature-section reveal">
      <div class="feature-section-header">
        <span class="ico">⚙️</span>
        <h2>Paramètres &amp; Thèmes</h2>
      </div>
      <ul class="feature-list">
        <li>7 thèmes de couleur : Navy · Red · Dark Green · Brown · Mustard · Salmon · Dark</li>
        <li>Thème "Dark" → mode sombre automatique</li>
        <li>Langue : Français / Anglais (mémorisé)</li>
        <li>Notifications globales on/off</li>
        <li>Profil utilisateur : nom, bio, téléphone, photo</li>
        <li>Fonctionnement hors-ligne (Firestore persistance illimitée)</li>
      </ul>
    </div>

    <!-- Stack technique -->
    <div class="feature-section reveal">
      <div class="feature-section-header">
        <span class="ico">🛠️</span>
        <h2>Stack technique</h2>
      </div>
      <div class="tech-grid">
        <div class="tech-item">
          <span class="tech-label">Framework</span>
          <span class="tech-value">Flutter 3.33 / Dart 3.7</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">Auth</span>
          <span class="tech-value">Firebase Authentication</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">Base de données</span>
          <span class="tech-value">Cloud Firestore</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">Stockage</span>
          <span class="tech-value">Firebase Storage</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">Push</span>
          <span class="tech-value">Firebase FCM</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">State</span>
          <span class="tech-value">Provider / ChangeNotifier</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">Carte</span>
          <span class="tech-value">Google Maps Flutter</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">Météo</span>
          <span class="tech-value">Open-Meteo API</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">PDF</span>
          <span class="tech-value">pdf + printing</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">Polices</span>
          <span class="tech-value">Playfair Display + Lato</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">Monitoring</span>
          <span class="tech-value">Crashlytics + App Check</span>
        </div>
        <div class="tech-item">
          <span class="tech-label">QR Code</span>
          <span class="tech-value">qr_flutter</span>
        </div>
      </div>
    </div>

  </div>
</section>

<!-- ═══ SCREENSHOTS ═══ -->
<section class="section section--dark">
  <div class="section-inner">
    <div class="section-header">
      <p class="eyebrow">Aperçu</p>
      <h2 class="section-title">L'application en images.</h2>
      <div class="gold-divider"><span></span></div>
    </div>
    <div class="gallery-wrap">
      <div class="gallery-grid">
        <div class="gallery-item reveal">
          <img src="screenshots/screenshot1.jpg" alt="Écran d'accueil">
          <div class="gallery-caption">Mes Voyages</div>
        </div>
        <div class="gallery-item reveal">
          <img src="screenshots/screenshot2.jpg" alt="Détail voyage">
          <div class="gallery-caption">Détail &amp; Onglets</div>
        </div>
        <div class="gallery-item reveal">
          <img src="screenshots/screenshot3.jpg" alt="Budget">
          <div class="gallery-caption">Finances</div>
        </div>
      </div>
    </div>
  </div>
</section>

<!-- ═══ CTA ═══ -->
<section class="download-section">
  <p class="eyebrow">Gratuit · iOS &amp; Android</p>
  <h2 class="section-title reveal">Téléchargez Ifenia dès maintenant.</h2>
  <div class="gold-divider"><span></span></div>
  <div class="store-badges reveal">
    <a href="https://play.google.com/store/apps/details?id=com.tangni.ifenia" class="badge-wrap" target="_blank" rel="noopener">
      <img src="assets/google-play-badge.jpg" alt="Google Play">
    </a>
    <a href="https://apps.apple.com/fr/app/ifenia/id6746134277" class="badge-wrap" target="_blank" rel="noopener">
      <img src="assets/app-store-badge.png" alt="App Store">
    </a>
  </div>
</section>
