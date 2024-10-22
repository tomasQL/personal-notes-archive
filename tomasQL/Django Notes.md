### Installing Django Framework

Linux / macOS

`python -m pip install Django`

Windows 
`py -m install Django`

Install the virtual enviroment

    python3 -m pip install --user virtualenv  
    
Setting up virutal enviroment






    python3 -m venv <folder name to the venv>
	    normally .venv or project name venv
    *add venv in file .gitignore
      
    source env/bin/activate  
    deactivate  


Creating a Django Project
	`$ django-admin startproject projectname`


Installing modules in folder project.

```
pip install djangorestframework
pip install markdown       # Markdown support for the browsable API.
pip install django-filter  # Filtering support
```

