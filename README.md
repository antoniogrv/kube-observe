<div align="center">
    <img align="center" src="https://kubernetes.io/images/nav_logo2.svg" alt="logo" width="300" />
    <h3>Kubernetes Observability & Detection Engineering</h3>
    <h4>Corso di Penetration Testing, a.a. 23/24, Università di Salerno</h4>
    <img align="center" src="https://raw.githubusercontent.com/antoniogrv/kube-observe/master/pictures/repo_cover.png" alt="logo" width="400" />
</div>

<hr />

Qualsiasi utente di [Kubernetes](https://kubernetes.io/it/docs/concepts/overview/what-is-kubernetes/) deve fare i conti con la sicurezza dei propri pod e del proprio cluster, a meno di applicativi estremamente semplici e poco affascinanti; capire come questa sicurezza può essere espletata, anche nella misura tale per cui ci si limita a *guardare* piuttosto che *agire*, è vitale alla compliance dovuta agli stakeholders e agli utenti del sistema.

Il corso di [Penetration Testing](https://docenti.unisa.it/026260/didattica?anno=2023&id=510980&cId=10000-2016&pId=N0*N0*S2), a cui questo progetto afferisce, insegna allo studente a scrutare una macchina virtuale, smembrarla, farla propria. Questa analisi, invece, punta ad illustrare *come capire che tutto questo sta accadendo*, e quali sono gli strumenti più adeguati per farlo; prima, però, viene descritto il funzionamento di un tipico cluster Kubernetes, anche correlandolo agli ambienti didattici di virtualizzazione implementati durante il corso; vengono, poi, opportunamente fornite alcune definizioni critiche per il contesto affrontato (fra cui **SIEM** e **SOAR**) e, infine, viene proposta una piccola sperimentazione esemplificativa.

In particolare, **la sperimentazione riguarda il bootstrap di un sistema SIEM su Kubernetes** usando strumenti allo stato dell’arte (i.e. [ELK](https://www.elastic.co/elastic-stack)). Questa sperimentazione afferisce, in parte o in tutto, ad una branca del DevOps Engineering e della Cybersecurity spesso indicata come "**Detection Engineering**", in cui si pone particolare accento sulla questione dell’osservabilità ("*[observability](https://www.ibm.com/it-it/topics/observability)"*). 

L’esigenza che un enorme cluster composto da centinaia di macchine virtuali e ospitante migliaia di applicativi debba essere osservabile (in una misura o nell’altra) potrebbe risultare scontata. Tuttavia, è facile dimenticare che il prezzo delle risorse (umane, economiche, computazionali) impiegate per realizzare sistemi di observability viene ripagato esclusivamente nei casi peggiori in cui questi sistemi arrivano a notificare disastri ed incidenti; fino ad allora, sembreranno non costituire alcun valore aggiunto. Ebbene, un incidente di sicurezza può davvero essere fatale per l’integrità e la confidenzialità dei dati, e per la disponibilità degli applicativi: fare in modo che questi ultimi siano costantemnete sotto l’occhio vigile di Kubernetes, a cui ne sarà delegata la governance e la mise-en-place, è il minimo che possiamo fare.
