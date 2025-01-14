.. _`§5`:

Richieste e risposte di autenticazione per la firma
===================================================

.. highlights:

   Sintassi dei messaggi SAML e JWT scambiati tra IdP e SP
   come parte del processo di autenticazione e di sottoscrizione.

La **richiesta di autenticazione** per la firma SPID, introdotta al
punto 5 della procedura di cui al §\ :ref:`3 <§3>`, contiene i seguenti metadati
aggiuntivi:

a. il nome del file del documento;

b. l’impronta dell’evidenza informatica ottenuta calcolando l’:ref:`impronta <hash>`
   del file di cui al punto a;

c. l’identificativo della funzione di *hash* crittografico utilizzato al
   punto b.

La **risposta di autenticazione** per la firma SPID contiene
obbligatoriamente i seguenti metadati:

d. il nome del file del documento firmato con SPID;

e. l’impronta dell’evidenza ottenuta calcolando l’impronta del file di
   cui al punto d, calcolata dall’IdP ai sensi del §\ :ref:`6 <§6>`;

f. l’identificativo della funzione di *hash* crittografico utilizzato al
   punto e.

L’identificativo unico della sessione di autenticazione (*session ID*)
di cui al §\ :ref:`3 <§3>`: punto 3, sempre presente in ogni richiesta e risposta di
autenticazione, associa in modo univoco il documento informatico
scambiato tra SP, IdP e vice versa, ad un’unica autenticazione di firma
SPID.

La durata delle sessioni di autenticazione descritte nell’ambito del
processo di sottoscrizione di cui alle presenti Linee guida è estesa
adeguatamente per permettere lo svolgimento dell’intera procedura di
sottoscrizione.

Le richieste e risposte di autenticazione per la firma SPID seguono la
sintassi descritta nei seguenti paragrafi.

.. toctree::
  :maxdepth: 3

  05/05.1_saml.rst
  05/05.2_secure-dataio.rst

.. discourse::

:topic_identifier: 666
