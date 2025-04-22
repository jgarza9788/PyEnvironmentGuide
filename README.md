# Create a virtual environment
```
python -m venv .\env_name
```

```
python -m venv .\env
```

```
python -3.10 -m venv .\env

```


# activate environment 
```bash
env\Scripts\activate
```

# deactivate 
```bash
deactivate
```

```
pipreqs . --force --encoding=utf8 --mode=gt
python -m venv .\env
.\env\Scripts\activate
pip install -r requirements.txt
```

```
pipreqs . --force --encoding=utf8 --mode=gt
C:\Users\JGarza\pythons\Python310\python.exe -m venv .\env
.\env\Scripts\activate
pip install -r requirements.txt
```


# at the top of python
```
try:
    import os
    import sys

    # Get the path to the virtual environment's activation script
    env_activate_path = os.path.join("env", "Scripts", "activate")

    # Check if the virtual environment exists and the OS is Windows
    if os.path.exists(env_activate_path) and sys.platform == "win32":
        # Execute the activation script
        activate_cmd = f'"{env_activate_path}"'
        os.system(activate_cmd)

    # Now you can continue with the rest of your script
    print("Virtual environment activated!")
except:
    print("unable to use virtual environment")
```