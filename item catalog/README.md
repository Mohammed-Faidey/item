Fixed issues

1- from flask import (
    Flask,
    render_template,
    request,
    redirect,
    jsonify,
    url_for,
    make_response,
    flash,
    session as login_session
)

2-modify clients_secrests.json file and add “javascript_origins”

2- vagrant/catalog/templates/login.html 1

modify data-clientid to become as in clients_secrests.json file


3- write README.md File 


4- vagrant/catalog/templates/item_new.html 1

use required attribute with input  in item_new.html file 
and 
in category_new.html file 


unfixed issues 
 -  at category_new.html and item_new.html how can I make  check to ensure that until a value is provided then users can submit the form 

## How do I run this?

### 1. Setup: Configure VM & Database

**Step 1:** Download and install [Vagrant](https://www.vagrantup.com/) and [VirtualBox](https://www.virtualbox.org). We’ll need these tools to setup and manage the Virtual Machine (VM). 


**Step 2:** Once you've cloned this project, open the terminal and then run the following commands:

```
# Install & Configure VM
cd /path/to/vagrant
vagrant up

# Log into machine
vagrant ssh

# Log out of machine
# <Ctrl + D>

# Destroy machine once done
vagrant destroy

```

Note: If this is the first time you're running [Vagrant Up](https://www.vagrantup.com/docs/cli/up.html) command, you need to wait a while after running the command. 


### 2. Run the website

Open the terminal. Then, run the following commands:

```
# Launch & Login to machine
cd /path/to/vagrant
vagrant up
vagrant ssh

# Open shared folder
cd /vagrant/catalog 

# Run the program
python catalog.py
```
