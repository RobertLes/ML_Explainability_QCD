# Template

# Install
```
python3.9 -m venv ~/venv/weaver
source ~/venv/weaver/bin/activate
pip install torch==1.13.1 h5py torchinfo numpy matplotlib scikit-learn weaver
pip install -r requirements.txt
```

Download datasets

There are many more samples available at https://opendata.cern.ch/record/80030, but downloading these two files is enough to get started with the training.

```
mkdir inputData
cd inputData
wget https://opendata.cern.ch/record/80030/files/assets/atlas/datascience/CERN-EP-2024-159/train_nominal_000.h5.gz
wget https://opendata.cern.ch/record/80030/files/assets/atlas/datascience/CERN-EP-2024-159/test_nominal_000.h5.gz
gunzip -f train_nominal_000.h5.gz
gunzip -f test_nominal_000.h5.gz
cd ..
```
