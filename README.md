# STARKNET-CAIRO-NFT

## Installation

Pour set-up votre environnement de développement :
Sur Mac si plusieurs versions de Python d'installé 💻

```bash

alias python3=python3.7
python3 -m venv cairo-venv
source cairo-venv/bin/activate
```
Au sinon
```bash
  python -m venv cairo-venv
source cairo-venv/bin/activate

// Linux
sudo apt install -y libgmp3-dev

// Mac (Intel chip)
brew install gmp 

// Mac M1
CFLAGS=-I`brew --prefix gmp`/include LDFLAGS=-L`brew --prefix gmp`/lib pip install ecdsa fastecdsa sympy

pip install --upgrade pip
# Installation de nile
pip install cairo-nile 
# Installation d'openzeppelin (import dans notre contract Cairo)
pip install openzeppelin-cairo-contracts
nile init
```
    
Compilation / déploiement du contract grâce au script run.py, modifier bien votre constructeur / le nom du contract dans celui-ci
```bash
nile run scripts/run.py --network goerli
```


