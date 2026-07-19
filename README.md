# Hyperparalelizer-2
Projeto de Sistemas Distribuídos

## Execução com 3 peers (rodar em terminais diferentes)
- **Coordenador**:    python -m main_beta4 server --host 127.0.0.1 --port 9000 --max-ram-mb 2048 --max-cpu-cores 2
- **Peer1**:           python -m main_beta4 peer --host 127.0.0.1 --port 9101 --server-port 9000 --max-ram-mb 512 --max-cpu-cores 1
- **Peer2**:           python -m main_beta4 peer --host 127.0.0.1 --port 9102 --server-port 9000 --max-ram-mb 512 --max-cpu-cores 1
- **Peer3**:           python -m main_beta4 peer --host 127.0.0.1 --port 9103 --server-port 9000 --max-ram-mb 512 --max-cpu-cores 1

### Atenção sobre Bug
A pasta data/ deve ser totalmente excluída antes de uma nova execução. A main.py faz isso, mas no caso de erros inesperados, **por favor se certifique que data/ está deletada**.