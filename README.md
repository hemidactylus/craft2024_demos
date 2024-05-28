# Vector Databases Demos

for the **Craft 2024** presentation.

## Setup

### Python environment

Ensure you are using Python v3.8 - v3.11 (newer versions _may_ work too).

Working in a virtual environment is suggested for isolation and better control.

Install

```
pip install -r requirements.txt
```

### Database

The happy path is to use an Astra DB instance to run the demos.

Visit `astra.datastax.com`, sign up for a free account, create a Vector Database
and when it's ready grab the _API Endpoint_ and generate a _Token_ for it.

### Secrets

Notebooks will ask you for these two secrets. If you're running locally, you can
copy the `.env.template` file to a new `.env` and set the secrets there to skip
interactive secret input. A few demos also need an OpenAI API key, which can also
be set in `.env`.

## Run the demos

Run locally from the repo's root with

```
jupyter notebook
```

or alternatively open the notebooks in Google Colab (links below).

**Note**. Free-tier accounts have a limited number of collections available.
If you run into an error ("too many indices...") while creating collections on
Astra DB, try dropping collections from previous demos. This means uncommenting
the actual `drop` method in each notebook's last cell -- just emptying the contents
with the `delete_all` method does not suffice).

### Demo 1 ("similarities on a sphere")

In the Jupyter console, open and run the **Demo 1** notebook.

Alternatively you can [run it in Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo1_Similarities_on_a_sphere.ipynb) (or just [view](demo1_Similarities_on_a_sphere.ipynb) the notebook).

### Demo 2 ("nearest spaceport")

Open and run the **Demo 2** notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo2_Nearest_spaceport.ipynb), or [view in browser](demo2_Nearest_spaceport.ipynb).

### Demo 3 ("mistyped philosophers")

Open and run the **Demo 3** notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo3_Mistyped_philosophers.ipynb), or [view in browser](demo3_Mistyped_philosophers.ipynb).

### Demo 4 ("similar 'products'")

Open and run the **Demo 4** notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo4_Similar_products.ipynb), or [view in browser](demo4_Similar_products.ipynb).

### Demo 5 ("sort your critters")

Open and run the **Demo 5** notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo6_Multi_vectors.ipynb), or [view in browser](demo6_Multi_vectors.ipynb).

### Demo 6 ("multi-vector search")

Open and run the **Demo 6** notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo6_Multi_vectors.ipynb), or [view in browser](demo6_Multi_vectors.ipynb).

### Demo 7 ("app migration")

Open and run the **Demo 7** notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo7_Migrate_app_Chroma_to_Astra.ipynb), or [view in browser](demo7_Migrate_app_Chroma_to_Astra.ipynb).

### Demo 8 ("text embeddings")

Open and run the **Demo 8** notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo8_Text_embeddings.ipynb), or [view in browser](demo8_Text_embeddings.ipynb).

**Note**: this demo will install additional requirements when run for the first time - an operation which may take a few minutes.

### Demo 9 ("philosophy quotes")

Open and run the **Demo 9** notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo9_Philosophical_Quotes.ipynb), or [view in browser](demo9_Philosophical_Quotes.ipynb).

**Note**: this demo is originally featured in the [OpenAI Cookbook](https://github.com/openai/openai-cookbook/tree/main/examples/vector_databases/cassandra_astradb#rag-with-astra-db-and-cassandra) gallery.
