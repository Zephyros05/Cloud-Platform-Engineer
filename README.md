# Cloud-Platform-Engineer
# Portfolio progetti Cloud e Terraform

Questa repository raccoglie i progetti più significativi realizzati durante il percorso di formazione in ambito cloud, infrastrutture e automazione. I lavori presenti mostrano competenze pratiche su Microsoft Azure, Terraform, PowerShell, Windows Server, networking e gestione dei servizi infrastrutturali.

L'obiettivo della repository è documentare progetti concreti sviluppati in laboratorio, con particolare attenzione alla progettazione modulare, all'automazione del deploy e alla risoluzione di problemi reali di configurazione e provisioning.

## Competenze principali

- Infrastructure as Code con Terraform.
- Deploy e configurazione di risorse su Microsoft Azure.
- Progettazione di reti virtuali, subnet e connettività tra macchine.
- Configurazione di macchine virtuali Windows e Linux.
- Automazione tramite PowerShell.
- Active Directory Domain Services e DNS.
- Azure Key Vault per la gestione sicura dei secret.
- Azure Storage Account, File Share, Blob, Queue e Table.
- Troubleshooting di errori di provisioning, timeout e dipendenze tra risorse.

## Progetti inclusi

### 1. Infrastruttura aziendale su Azure con Terraform

Progettazione e realizzazione di un'infrastruttura completa su Microsoft Azure per simulare un ambiente aziendale, composta da Domain Controller, File Server, Web Server, VPN Gateway, Key Vault e Azure File Share.

Il progetto è stato automatizzato con Terraform e organizzato in moduli per rete, macchine virtuali, storage, sicurezza e connettività. Sono stati sviluppati script PowerShell per la creazione del dominio Active Directory, il join delle macchine al dominio e l'installazione automatica di IIS.

Tra gli aspetti più rilevanti del progetto:
- creazione di una Virtual Network con subnet separate per i diversi servizi;
- configurazione di VM Windows con ruoli distinti;
- utilizzo di Azure Key Vault per la gestione delle password;
- montaggio di una Azure File Share come unità di rete;
- pubblicazione di un sito statico su IIS;
- configurazione di una VPN per l'accesso remoto alle risorse private.

Questo progetto ha richiesto attività di troubleshooting reale su errori di memoria, timeout delle VM extension, riavvii durante il provisioning e gestione delle dipendenze tra risorse.

**Tecnologie utilizzate:** Terraform, Microsoft Azure, PowerShell, Windows Server, Active Directory, IIS, Azure Key Vault, Azure Storage, VPN Gateway.

### 2. Automazione di Active Directory su Windows Server

Sviluppo di script PowerShell per installare e configurare automaticamente Active Directory Domain Services su Windows Server, con creazione della foresta, configurazione del dominio e join automatico delle macchine al dominio.

L'attività ha incluso l'integrazione con Azure Custom Script Extension e la gestione di problematiche legate a tempi di esecuzione, reboot della macchina e stabilità del provisioning.

**Tecnologie utilizzate:** PowerShell, Windows Server, Active Directory Domain Services, DNS, Azure VM Extension.

### 3. Deploy modulare di infrastrutture con Terraform

Realizzazione di progetti Terraform organizzati in moduli riutilizzabili per separare rete, macchine virtuali, storage e sicurezza. Questa struttura ha permesso di mantenere il codice più leggibile, scalabile e semplice da correggere o ampliare.

Sono stati gestiti input, output, variabili condivise, dipendenze tra moduli e state Terraform, con attenzione alla ripetibilità del deploy e alla qualità dell'organizzazione del progetto.

**Tecnologie utilizzate:** Terraform, AzureRM Provider, moduli Terraform, Infrastructure as Code.

### 4. Progetto Azure Storage e gestione dati

Creazione e configurazione di risorse di storage su Azure, tra cui Storage Account, File Share, Blob Container, Queue e Table. Il progetto ha incluso il caricamento di file, il montaggio di share su macchina virtuale e l'esplorazione delle risorse tramite Azure Storage Explorer.

Questo lavoro ha permesso di approfondire la gestione pratica dei servizi di archiviazione cloud e delle diverse modalità di accesso ai dati.

**Tecnologie utilizzate:** Microsoft Azure, Terraform, Azure Storage Account, Blob Storage, File Share, Queue, Table, Azure Storage Explorer.

### 5. Deploy di macchine virtuali Linux e Windows nella stessa rete

Realizzazione di un progetto Terraform per distribuire una macchina Linux e una macchina Windows Server in subnet separate della stessa Virtual Network, con relative interfacce di rete, regole di sicurezza e test di connettività tra le VM.

Il progetto è stato utile per consolidare i concetti di networking su Azure, organizzazione modulare del codice e differenze di configurazione tra sistemi operativi diversi.

**Tecnologie utilizzate:** Terraform, Azure Virtual Network, NSG, Linux VM, Windows Server VM.

## Approccio di lavoro

I progetti sono stati sviluppati seguendo un approccio pratico orientato a:
- modularità del codice;
- automazione delle attività ripetitive;
- chiarezza nella struttura delle cartelle e dei file;
- attenzione alla sicurezza nella gestione delle credenziali;
- verifica finale del corretto funzionamento delle risorse distribuite.

Una parte importante del lavoro è stata dedicata al troubleshooting, cioè all'analisi e alla correzione di errori reali emersi durante il deploy. Questo ha permesso di acquisire esperienza concreta non solo nella creazione delle risorse, ma anche nella loro validazione e nel loro ripristino in caso di problemi.

## Obiettivo della repository

Questa repository rappresenta una raccolta di progetti pratici sviluppati per consolidare competenze in ambito cloud e infrastrutturale. L'insieme dei lavori mostra una crescita progressiva nell'uso di Terraform, Azure e strumenti di automazione, con attenzione sia agli aspetti tecnici sia all'organizzazione professionale dei progetti.

