## 💾 Archivní Projekt: Vagrant, Nginx, HAProxy Load Balancer a Zabbix Monitoring

Tento repozitář obsahuje archiv řešení mého vysokoškolského projektu zaměřeného na nasazení a monitorování distribuované služby.

### 📋 Popis Projektu

Cílem projektu bylo vytvořit prostředí zahrnující:

* **Vagrant:** Pro automatizované vytvoření a správu virtuálních strojů.
* **Nginx:** Jako webový server na back-end uzlech.
* **HAProxy:** Jako **software load balancer** pro distribuci zátěže mezi Nginx servery.
* **Zabbix:** Pro **monitorování** stavu celého systému, vrátane uzlů a služeb.

---

### ⚠️ Upozornění - Důležité!

> [!CAUTION]
> **Tento repozitář slouží čistě jako ARCHIVACE mé dřívější práce.**

* Projekt byl vyvinut v rámci specifického studijního zadání a nemusí reprezentovat současné **best practices** nebo být plně v souladu s dnešními verzemi softwaru.
* **Funkčnost negarantována:** Kvůli zastaralým verzím Vagrant boxů, závislostí, nebo změnám v konfiguraci operačních systémů, není zaručeno, že po klonování a spuštění projekt **okamžitě a správně funguje**.
* Je zde uložen primárně pro účely **dokumentace, revize kódu a uchování historie mého akademického vývoje**.

### 💻 Struktura

Projekt obsahuje soubory pro:

* `Vagrantfile`: Hlavní konfigurační soubor pro virtuální stroje.
* Konfigurační soubory pro Nginx, HAProxy a Zabbix (např. v adresáři `konfigurace/`.
* Skripty pro automatické zprovoznění.
