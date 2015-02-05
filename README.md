# it394_project_template
A project template for a Python/Django project ready to deply into the Heroku production environment.

# How to use this template
To use this template start a new project using django-admin and the --template parameter
```
django-admin startproject --template=http://github.com/usma-it394/it394_project_template/archive/master.zip <project name>
```
django-admin startproject will correctly rename the project_name folder and also replace the {{ }} patterns with the correct values in the project_name folder.

Unfortunately, it does not apply changes to the root directory of the project.  I've included a simple PowerShell script named "fix_project_name.ps1" that will replace the {{ project_name }} pattern in the root directory.  So after you start the project run
```
fix_project_name -name "project name"
```

