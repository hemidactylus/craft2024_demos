# Vector Databases Demos

for the **Craft 2024** presentation.

## Setup

### Python environment

Ensure you are using Python v3.8 - v3.10 (newer versions _may_ work too).

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
copy the `.env.template` file to a new `.env` and set the secrets there.

## Run the demos

Run locally from the repo's root with

```
jupyter notebook
```

or alternatively open the notebooks in Google Colab (links below).

**Note**. Free-tier accounts have a limited number of collections available.
If you run into an error ("too many indices...") while creating collections on
Astra DB, try dropping collections from previous demos (actual `drop` method;
just emptying the contents does not suffice).

### Demo 1 ("similarities on a sphere")

In the Jupyter console, open the **Demo 1** folder and then run the notebook.

Alternatively you can [run it in Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo1_similarities_on_a_sphere/Similarities_on_a_sphere.ipynb) (or just [view](demo1_similarities_on_a_sphere/Similarities_on_a_sphere.ipynb) the notebook).

### Demo 2 ("nearest spaceport")

Open the **Demo 2** folder and run the notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo2_nearest_spaceport/Nearest_spaceport.ipynb), or [view in browser](demo2_nearest_spaceport/Nearest_spaceport.ipynb).

### Demo 3 ("mistyped philosophers")

Open the **Demo 3** folder and run the notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo3_mistyped_philosophers/Mistyped_philosophers.ipynb), or [view in browser](demo3_mistyped_philosophers/Mistyped_philosophers.ipynb).

### Demo 4 ("similar 'products'")

Open the **Demo 4** folder and run the notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo4_similar_products/Similar_products.ipynb), or [view in browser](demo4_similar_products/Similar_products.ipynb).

### Demo 5 ("sort your critters")

Open the **Demo 5** folder and run the notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo6_multi_vectors/Multi_vectors.ipynb), or [view in browser](demo6_multi_vectors/Multi_vectors.ipynb).

### Demo 6 ("multi-vector search")

Open the **Demo 6** folder and run the notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo6_multi_vectors/Multi_vectors.ipynb), or [view in browser](demo6_multi_vectors/Multi_vectors.ipynb).

### Demo 7 ("app migration")

Open the **Demo 7** folder and run the notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo7_app_migration/Migrate_app_Chroma_to_Astra.ipynb), or [view in browser](demo7_app_migration/Migrate_app_Chroma_to_Astra.ipynb).

### Demo 8 ("text embeddings")

Open the **Demo 8** folder and run the notebook.

Alternatively: [Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo8_vector_embeddings/Text_embeddings.ipynb), or [view in browser](demo8_vector_embeddings/Text_embeddings.ipynb).

**Note**: this demo will install additional requirements when run for the first time - an operation which may take a few minutes.
