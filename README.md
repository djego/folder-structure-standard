Folder Structure Standar
============================

> Folder structure standar for software projects

### Top-level directory layout

    ├── src/                     # Source files 
    ├── container/               # Docker files 
    ├── deploy/                  # Deploy files
    ├── doc/                     # Documentation files 
    ├── test/                    # Automated tests files 
    ├── Makefile
    ├── CHANGELOG.md
    └── README.md

> Use short lowercase names at least for the top-level files and folders except
> `Makefile`, `README.md`

## Source files

In `src` folder you can add the code of your application for example: 
- Rails project: app, lib, config, db and more.
- Django project: apps, manage.py and more.
- Spring project: src/main, pom.xml and more.
- React project: src, public, package.json and more.

## Docker files 
In `container` folder you can add configuration files associate with your containers and local development.

## Deploy files 
In `deploy` folder you can add configuration files associate with your delivery process.  

> Also in this folder you might to add `IaaC` files as sub module 
> 
## Documentation files

In `doc` folder you can add information about your project for example usage.md for explain how to use your app, raml for api documentation. 

> Often it is beneficial to include some reference data into the project, such as Rich Text Format (RTF) documentation, which is usually stored into the `docs`
or, less commonly, into the `doc` folder.

### Layout  
    ├── ...
    ├── doc                    # Documentation files
    │   ├── erd.md              # Entities relation database
    │   ├── usage.md            # How to use 
    │   ├── raml                # API documentation
    │   └── ...                 # etc.
    └── ...


## Automated tests

In `test` folder you can add the differents tests of your aplication. 

> **Q: Why tests are placed into a separate folder, as opposed to having them closer to the code under test?**
>
> **A:** Because you don't want to test the code, you want to test the *program*.

### Layout 

    ├── ...
    ├── test                    # Test files
    │   ├── benchmarks          # Load and stress tests
    │   ├── integration         # End-to-end, integration tests
    │   └── unit                # Unit tests
    └── ...

