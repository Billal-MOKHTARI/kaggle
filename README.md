# kaggle

## Set kaggle environement in python

```shell
pip install -q kaggle
mkdir ~/.kaggle
cp kaggle.json ~/.kaggle/
chmod 600 ~/.kaggle/kaggle.json
kaggle datasets list
kaggle datasets download 'name-of-competition'
unzip file.zip -d folder
```

```python
def load_files(dataset, folder=PATH_DATA):
  os.system('pip install -q kaggle')
  files.upload()
  os.system('mkdir ~/.kaggle')
  os.system('cp kaggle.json ~/.kaggle/')
  os.system('chmod 600 ~/.kaggle/kaggle.json')
  os.system("kaggle datasets download  '"+dataset+"'")
  os.system("mkdir data")
  file = dataset.split('/')[-1]+'.zip'
  os.system('unzip '+file+' -d '+folder)
  os.system('rm -r '+file)
  ```
