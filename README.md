# NLP_text_classification

Il progetto assegnato richiede la creazione di un dataset sintetico contenente almeno $1000$ esempi di testo da utilizzare per estrarre in modo automatizzato delle classi (anche chiamate label o categorie). 
La soluzione proposta si articola in due parti principali:
1. La creazione del dataset sintetico utilizza GPT-2 un modello di linguaggio generativo che partendo da un prompt genera un output testuale generalmente coerente.
2. L'estrazione delle varie classi utilizza una tecnica di topic modelling chiamata Latent Dirichlet Allocation (LDA) capace di estrarre in modo non supervisionato delle classi partendo da input testuali. 

Il progetto è interamente sviluppato in Python utilizzando librerie che implementano funzionalità dedicate al natural language processing quali Scikit-learn, Hugging Face Transformers. 

## Descrizione della repository

Il file `env.yml` contiene tutte le librerie necessarie per eseguire il codice. Per installarle è sufficiente eseguire il comando 

`conda env create -f env.yml`.

Il codice per generare il dataset sintetico è contenuto nel notebook `Dataset_generation.ipynb`. Il codice per estrarre le classi dal dataset è contenuto nel notebook `Topic_modelling.ipynb`.

La cartella `dataset` contiene il dataset sintetico generato e la cartella `model` contiene i modelli utilizzati per l'estrazione delle classi.