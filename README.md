# CATS2D: CATS2D descriptor generator with RDKit
rdkit_cats2d
- Original work
  - http://www.rguha.net/code/python/cats2d.py
  - https://github.com/arthuc01/RDKit-Cats2D


## Requirements
- RDKit
- Numpy


## Install CATS2D

    git clone https://github.com/iwatobipen/CATS2D.git
    cd CATS2D
    pip install -e .


## Usage

    from rdkit import Chem
    from cats2d.rd_cats2d import CATS2D
    cats = CATS2D()
    mol = Chem.MolFromSmiles('COCC')
    cats.getCATs2D(mol)         