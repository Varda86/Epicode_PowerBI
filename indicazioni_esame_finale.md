# Epicode_PowerBI_project
 final practice of Power BI module


Scenario
Olist store è un sito di e-commerce brasiliano per seller (venditori).
La piattaforma consente ai seller di proporre i propri prodotti ai diversi mercati brasiliani.
Il dataset pubblico (e anonimizzato) espone gli ordini di vendita dal 2016 al 2018 e consente di quantificarli, misurarli, analizzarsi rispetto dimensioni di analisi diverse: cliente, prodotto, metodi di pagamento, status dell’ordine, …
Obiettivi di analisi
È necessario sviluppare un report di BI che consenta di analizzare:
1.	L’andamento degli ordini nel tempo per stato (geografico)*
2.	L’andamento dei ricavi nel tempo per stato**
3.	Distribuzione del rating***
*l’utente, dato un particolare anno selezionato, vorrebbe poter visualizzare il conteggio degli ordini mese per mese. Inoltre, vorrebbe poter confrontare i risultati con quelli dell’anno precedente e, rispetto a questi, visualizzare la variazione percentuale mese per mese. È fondamentale poter filtrare rispetto allo status dell’ordine (ad esempio delivered, shipped, …).
Il campo da considerare per il conteggio degli ordini è olist_order_items_dataset|order_item_id.
Per i dati geografici bisogna fare riferimento al campo olist_customers_dataset|customer_state.
Per applicare il filtro sullo status degli ordini utilizza il campo olist_orders_dataset|order_status.
** l’utente, dato un particolare anno selezionato, vorrebbe poter visualizzare i ricavi totali mese per mese. Inoltre, vorrebbe poter confrontare i risultati con quelli dell’anno precedente e, rispetto a questi, visualizzare la variazione percentuale mese per mese. È fondamentale poter filtrare rispetto allo status dell’ordine (ad esempio delivered, shipped, …).
Per calcolare il ricavo della singola transazione è necessario considerare la somma di olist_order_items_dataset|price e olist_order_items_dataset|freight_value cioè la somma del prezzo di vendita e del costo di spedizione/consegna.
***utilizza il campo olist_order_reviews_dataset|review_score. 
 Applica tutte le best practice condivise:
1.	Riduci il volume del dataset
2.	Ristruttura i dati grezzi in modo tale da ottenere uno star schema
3.	Utilizza una dimensione calendario
4.	Progetta un buon layout 
5.	Progetta una buona UX (tooltip, bottoni, drill-through per esporre maggiori livelli di dettaglio rispetto a certe aggregazioni...)
6.	Arricchisci il report anche di altre analisi: distribuzione del rating (utilizza la tabella olist_order_reviews_dataset, analisi per prodotto e/o per area geografica.


Tip
Le tabelle strettamente necessarie alle analisi sono: 
	olist_orders_dataset
	olist_order_items_dataset
	olist_products_dataset
	olist_order_reviews_dataset
	olist_customers_dataset
Nota bene: ti viene fornita l’estrazione dati completa per tua comodità qualora tu volessi approfondire per tuo esercizio lo scenario proposto. 



