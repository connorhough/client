# Weights & Biases's documentation

This package provides an interactive CLI and python client for [wandb.ai](https://app.wandb.ai).

## Quickstart

If you want to work with private buckets or push data to the cloud you must first [signup](https://app.wandb.ai/login)

```console
$ pip install wandb
$ cd my_training_dir
$ wandb init
$ ./my_training_script.py arg1 arg2 | wandb my_bucket model.json weights.h5
```

To manually push files to the cloud run:

```console
$ wandb push my-new-bucket somefile.pb
```

To pull down a public model or sync your local directory with the cloud you can run:

```console
$ wandb pull zoo/inception_v4
```

Or you can pull directly in a python script:

```python
import wandb
client = wandb.Api()
client.pull("zoo/inception")
```

## Documentation

```eval_rst
.. toctree::
   :maxdepth: 4

   installation
   usage
   wandb
```
   
## Reference

```eval_rst
* :ref:`genindex`
* :ref:`modindex`
* :ref:`search`
```