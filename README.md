# FabMechanics


## How to contribute
### Installation locally (not docker)

Install UV as package manager
```sh
curl -LsSf https://astral.sh/uv/install.sh | sh
```
Install Python 3.13.2 and create the virtual environment
```sh
uv python install 3.13.2
uv venv --python 3.13.2
```

Install the dependencies
```sh
source .venv/bin/activate
uv sync
```

Run mkdocs locally
```sh
mkdocks serve
```

