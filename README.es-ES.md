<div align="center">

# Infundir la Auto-consistencia en la Predicción del Hamiltoniano de la Teoría de la Funcional de la Densidad mediante Modelos de Equilibrio Profundo


[![python](https://img.shields.io/badge/-Python_3.7_%7C_3.8_%7C_3.9_%7C_3.10-blue?logo=python&logoColor=white)](https://github.com/pre-commit/pre-commit)
[![pyg](https://img.shields.io/badge/-pyg_2.3.0-34e1e9)](https://pytorch-geometric.readthedocs.io/en/latest/#)



</div>

## 📌 Introducción

Infundir la Auto-consistencia en la Predicción del Hamiltoniano de la Teoría de la Funcional de la Densidad mediante Modelos de Equilibrio Profundo.


## 🚀 Puesta en Marcha Rápida

Instalar dependencias

```bash
# clonar el proyecto
git clone https://github.com/Zun-Wang/DEQHNet.git
cd DEQHNet

# [OPCIONAL] crear entorno conda
[Opcional] conda create -n DEQHNet python=3.10
[Opcional] conda activate DEQHNet

# Recomendar instalar parte de las dependencias por adelantado
# Tomar como ejemplo la versión `cuda121`
pip install torch==2.1.2 --index-url https://download.pytorch.org/whl/cu121
pip install pyg_lib torch_scatter torch_sparse torch_cluster torch_spline_conv -f https://data.pyg.org/whl/torch-2.1.0+cu121.html
pip install torch_geometric==2.3.0

pip install pytorch-lightning==1.8.3

pip install pyscf==2.2.1
conda install psi4 python=3.9 -c conda-forge

pip install requirements.txt

pip install -e .
```

Entrenar DEQHNet, por ejemplo: 
```bash
cp auxiliary.gbs src/QHNet/
cd src/QHNet/
set basis AUXILIARY
python src/QHNet/train_wH.py dataset=uracil model=QHNet model.version=DEQHNet
```


## Cita
```
@inproceedings{wang2024infusing,
  title={Infundir la Auto-consistencia en la Predicción del Hamiltoniano de la Teoría de la Funcional de la Densidad mediante Modelos de Equilibrio Profundo},
  author={Wang, Zun and Liu, Chang and Zou, Nianlong and Zhang, He and Wei, Xinran and Huang, Lin and Wu, Lijun and Shao, Bin},
  booktitle={The Thirty-eighth Annual Conference on Neural Information Processing Systems},
  year={2024},
  url={https://openreview.net/forum?id=PSVkinBs4u}
}
```


## Agradecimientos
Este proyecto se basa en el repo [AIRS](https://github.com/divelab/AIRS.git).
