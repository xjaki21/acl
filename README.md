# ACL — Access Control List

Una web application gestionale sviluppata in **PHP** per la gestione di permessi e ruoli utente (Access Control List). Il progetto è strutturato con una separazione netta tra frontend, backend e database, e supporta il deploy tramite **Docker**.

---

## Struttura del progetto

```
acl/
├── BACK END/           # Logica server-side in PHP
├── FRONT END/          # Interfaccia utente (HTML, CSS)
├── DATABASE/           # Script SQL e configurazione del database
├── PROJECT MANAGEMENT/ # Documentazione e gestione del progetto
├── index.php           # Entry point dell'applicazione
├── Dockerfile          # Configurazione immagine Docker
└── docker-compose.yml  # Orchestrazione dei servizi
```

---

## Tecnologie utilizzate

- **PHP** — logica backend e gestione delle ACL
- **CSS** — stile e layout dell'interfaccia
- **MySQL / MariaDB** — database relazionale
- **Docker / Docker Compose** — containerizzazione e deploy

---

## Avvio con Docker

### Prerequisiti

- [Docker](https://www.docker.com/) installato
- [Docker Compose](https://docs.docker.com/compose/) installato

### Istruzioni

1. **Clona la repository:**

   ```bash
   git clone https://github.com/xjaki21/acl.git
   cd acl
   ```

2. **Avvia i container:**

   ```bash
   docker-compose up -d
   ```

3. **Apri il browser e vai su:**

   ```
   http://localhost
   ```

4. **Per fermare i container:**

   ```bash
   docker-compose down
   ```

---

## Configurazione del database

Gli script SQL per la creazione e il popolamento del database si trovano nella cartella `DATABASE/`. Assicurati di eseguirli dopo aver avviato i container, o verifica se sono già inclusi nell'avvio automatico tramite Docker Compose.

---

## Funzionalità principali

- Gestione **utenti** e **ruoli**
- Definizione di **permessi** granulari per risorsa
- Pannello di amministrazione per la configurazione delle ACL
- Interfaccia web responsive

---

## Licenza

Questo progetto è distribuito senza una licenza esplicita. Contatta l'autore per informazioni sull'utilizzo.

---
