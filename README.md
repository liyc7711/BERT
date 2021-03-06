# BERT
a simple yet complete implementation of the popular BERT model.

Experiments show this code could achieve close performance to that of Google.

## Advanced Features
- Distributed training
- Lazy file reader

## Quick Guide
- This code is very simple, it should explain itself.
- Distributed training settings
  - --world_size #total number of gpus
  - --gpus #gpus on this machine
  - --MASTER_ADDR #master node IP
  - --MASTER_PORT #master node port
  - --start_rank # range from 0 to world_size-1, the index of the first gpu on this machine
  - --backend # 'nccl' or 'gloo', nccl is generally better but may not work on some machines
- Exemplar use of a trained model
  - See `example_use.py` and `example_use.sh` for more details
