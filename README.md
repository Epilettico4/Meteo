# Meteo

#Funzionalità
L’applicazione web permette di:
  Visualizzare una mappa interattiva tramite Leaflet.
  Cliccare sulla mappa per registrare un nuovo punto.
  Ottenere automaticamente:
    latitudine e longitudine cliccate,
    nome della località tramite Nominatim (reverse geocoding),
    temperatura attuale tramite Open-Meteo.
  Salvare ogni punto su PocketBase (lat, lon, descrizione, temperatura).
  Visualizzare sulla mappa tutti i marker già salvati all’avvio.
  Mostrare statistiche: numero punti, temperatura media, minima e massima.
  Aggiornare le temperature di tutti i punti tramite pulsante dedicato.
  Applicare una legenda colori in base alla temperatura.

#tecnologie utilizzate
  Vite
    Bundler e dev-server moderno.
    Avvio rapido, hot reload e gestione semplice dei moduli ES.
    Utilizzato per costruire e servire l’applicazione.
  Leaflet.js
    Libreria leggera per mappe interattive.
    Usata per:
      visualizzare la mappa,
      gestire gli eventi di click,
      creare marker e popup.
  PocketBase
    Database locale + API REST + autenticazione.
    Usato per:
      salvare i punti registrati,
      recuperare i record all’avvio,
      aggiornare i dati (temperatura).
  Open-Meteo API
    API pubblica di meteo in tempo reale.
    Fornisce la temperatura attuale per una coppia di coordinate.
  Nominatim (OSM) API
    Servizio di reverse geocoding.
    Converte coordinate → nome del luogo.
