# snakemake-pixi

Building snakemake workflows with pixi ✨

## Installation

The following commands install dependencies of the workflow in the _current_
directory within the `.pixi` folder. After installation, you cannot move the
folder without re-installling all the dependencies. 

```bash
curl -fsSL https://pixi.sh/install.sh | bash
# ... cd <this repo>
pixi install
```

## Usage

* `pixi run make` runs the full workflow. You can supply arguments to `snakemake` as needed, such as `--cores 10`, if your process needs 10 cores.

* `pixi run test` runs a dry run (`-np`) of the workflow. 

* `pixi run update_dag` updates the directed acyclic graph of the snakemake workflow and moves it to the `resources` folder.

* `pixi run help` show the usage of the Snakefile
