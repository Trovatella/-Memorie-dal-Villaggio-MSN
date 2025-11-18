**Il Giudizio del Kernel sulle Chiavi di Telegram 🔴🔨🎓📚**


**Dal Vangelo di San Root e San Log**


<div style="text-align:center; margin:20px 0;">
  <div style="display:inline-block; max-width:360px; width:100%; border:3px solid #4b0082; border-radius:10px; padding:10px; background:linear-gradient(135deg,#1e3a8a,#4b0082); box-shadow:0 3px 10px rgba(0,0,0,0.3);">
    
    <div style="font-family:monospace; font-size:16px; color:#facc15; margin-bottom:8px; text-align:center; text-shadow:0 0 5px #000;">
      🗝️ Keeper of the Seven Keys ⚔️
    </div>
    
    <div style="position:relative; padding-top:56.25%; border-radius:6px; overflow:hidden;">
      <iframe
        src="https://www.youtube.com/embed/sOnrRFd3Juk"
        title="Helloween – Keeper of the Seven Keys"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen
        style="position:absolute; top:0; left:0; width:100%; height:100%; border:0;">
      </iframe>
    </div> 
    
  </div>
</div>




🐧Prologo: Il secondo giorno del Reboot

 “Nel tempo in cui i pacchetti venivano sniffati e le chiavi scambiate in chiaro, il Kernel osservava in silenzio.”

Un vento di aggiornamento soffiò tra le righe del codice. Le comunità, già divise tra CLI e GUI, iniziarono a farsi domande: chi aveva davvero il controllo delle chiavi? Chi firmava i certificati del Villaggio?

---
E fu **Telegram** con derivazioni di Java e tecniche trafugate nell'ombra del C++ a decantare tutta la folla. 

🤡 Furono i nuovi falsi profeti: tra API e illusioni
**Telegram**, già evocato nel primo cantico, si moltiplicava in fork e in bot.  
Ma ora giungevano nuovi falsi profeti:  
- Il Profeta di Signal, che prometteva silenzio assoluto.  
- Il Profeta di Matrix, che parlava in federazioni.  
- Il Profeta di Session, che non voleva nemmeno sapere chi sei.

Ma il Kernel non dimentica.  
Ogni chiave è una promessa. Ogni fork è una tentazione.
---
**I profeti di Telegram vennero giudicati**

Di quali peccati è colpevole **Telegram** 
Che tutte le chats lascia in chiaro 
Esfiltra le chat segrete
E fughe di dati provoca! 

Così tuonando dall'abisso del CLI
Una voce divina si stagliò feroce 
Contro il popolo:

L'ira di KERNEL:

Dai Sysadmin Apostoli

"I peccati di Telegram sono:
l'uso **non standard di AES**: 

Telegram utilizza AES‑256 in modalità IGE (Infinite Garble Extension), 
una modalità poco diffusa e considerata fragile rispetto a CTR o GCM. Questo ha sollevato dubbi sulla robustezza del protocollo.
  
**La gestione delle chiavi**:

 Le chiavi di sessione vengono generate e gestite dai server Telegram, non in modo end‑to‑end tra utenti. 
 Questo significa che Telegram ha accesso alle chiavi e può, in teoria, decifrare i messaggi. "
 

" E" aggiunse San Vim 
"Abusò anche di Kotlin"
Anche San Patch ne fu testimone e così gli Apostoli parlarono:

"Telegram abusa di **Kotlin** eseguendo codice monolitico e poco idiomatico, che sfrutta Kotlin come “Java travestito” invece che come linguaggio moderno.  

E poi abusa di coroutines senza strutture di cancellazione o gestione corretta degli scope, con rischi di memory leak.  
  
I Layer crittografia sono sì scritti in Kotlin ma con logica derivata da C++ /Java, creando incoerenze e bug.  

E infine le dipendenze non se sono modulari: invece di sfruttare la modularità di Kotlin, Telegram ha mantenuto un approccio centralizzato che rende difficile la manutenzione.  

E fu così che Telegram, nel suo MTProto, confuse le chiavi dell’AES‑256:  
non in GCM né in CTR, ma in IGE, fragile e dimenticato.  
Le sessioni firmate dal server, non dagli uomini,  
rivelarono che ogni promessa di segretezza era solo un'illusione.  
Telegram abusò di Kotlin:  
travestì Java con nuove coroutines,  
 ma dimenticò gli scope e le chiavi,  
lasciando il Villaggio in balia di leak e illusioni.”  


🐧🎓Il Giudizio del Kernel
“Tu che hai chmodato il mondo, ora giudica le permissioni degli uomini.”

Il Kernel parlò:  
- Chi usa sudo senza sapere, sarà ignorato.  
- Chi firma con chiavi generate da terzi, sarà osservato.  
- Chi archivia senza fare backup, verrà dimenticato.

