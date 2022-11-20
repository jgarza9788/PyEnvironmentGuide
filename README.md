
### Environments and Packages
these are some python commands to create and use environments


create an environment
```CMD
conda create -n <NAME> python=<version>
```
deleting environment
```CMD
conda env remove -n ENV_NAME
```
activate an environemtn
```CMD
activate <NAME> 
```
deactivate an environemtn
```CMD
deactivate <NAME> 
```
freeze an environemtn
```CMD
conda env freeze <NAME>
```
better freeze
```
pipreqs . --force
```


list environments
```CMD
conda info --envs
```
Install packages
```CMD
conda install PACKAGE_NAME
```
remove package
```CMD
conda remove PACKAGE_NAME
```
update package
```CMD
conda update package_name
```
search packages
```CMD
conda search '*beautifulsoup*'
```
list packages
```CMD
conda list
```
create and add packages to environment
```CMD
conda create -n env_name [python=X.X] [LIST_OF_PACKAGES]
```
exporting environment
```CMD
conda env export
```
```CMD
conda env export > environment.yaml
```
```CMD
conda env create -f environment.yaml 
######## create an environment with the name environment.yaml
```