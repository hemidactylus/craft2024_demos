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

### Demo 1 ("similarities on a sphere")

In the Jupyter console, open the **Demo 1** folder and then run the notebook.

Alternatively you can [run it in Colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo1_similarities_on_a_sphere/Similarities_on_a_sphere.ipynb) (or just [view](demo1_similarities_on_a_sphere/Similarities_on_a_sphere.ipynb) the notebook).

### Demo 2 ("counter/examples")

Open the **Demo 2** folder and run the desired notebook.

A - nearest_spaceport: [colab](https://colab.research.google.com/github/hemidactylus/craft2024_demos/blob/main/demo2_vectors_counter_examples/A_nearest_spaceport.ipynb), [view in browser](demo2_vectors_counter_examples/A_nearest_spaceport.ipynb).
