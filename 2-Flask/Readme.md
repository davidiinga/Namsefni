### Hvað er Flask

[Flask](https://flask.palletsprojects.com/en/2.1.x/) (source code) is a Python web framework built with a small core and easy-to-extend philosophy. 

Flask is considered more Pythonic than the Django web framework because in common situations the equivalent Flask web application is more explicit. Flask is also easy to get started with as a beginner because there is little boilerplate code for getting a simple app up and running. [Flask – Overview](https://www.tutorialspoint.com/flask/flask_quick_guide.htm)

- [Leiðbeiningar: Flask Uppsetning](Flask-Uppsetning.md)
- [Uppsetningar vandamál](Vandamal.md)


#### Uppsetning á Flask

- https://flask.palletsprojects.com/en/1.1.x/installation/

<!--
### Skoða betur linka (kennari)
- https://vefthroun.github.io/Verkefni-1/vefthroun.html
- http://www.compjour.org/lessons/flask-single-page/hello-tiny-flask-app/
- https://pythonbasics.org/flask-tutorial-hello-world/
- [Flask Mega Tutorial](https://blog.miguelgrinberg.com/post/the-flask-mega-tutorial-part-i-hello-world)
- Flask by Example – Project Setup https://realpython.com/flask-by-example-part-1-project-setup/
-->

---

#### Windows leiðbeiningar (með notkun power shell)
1. Þú þarft að hafa nýlega stöðuga (stble) útgáfu t.d. 3.8.x af [python þýðanda](https://www.python.org/downloads/release/python-387/).
    1. Til að kanna núverandi útgáfu:  `python --version` 
1. Virutal environment
    1. búðu til möppu t.d. vefur3 í tölvunni t.d. á C: rót: `mkdir vefur3`
    1. færðu þig í vefur3 möppuna `cd vefur3`
    1. settu upp virtual venv: `py -3 -m venv venv`
    1. activate venv: `venv\Scripts\activate`
1. Install flask framework 
    1. Activate venv: `venv\Scripts\activate`
    1. Notaðu pip til að install flask: `pip install flask`
    1. Opnaðu python þýðandann: `python`            
    1. Athugaðu hvort flask hafi installast:  `>>> import flask`  
    1. ef það er engin villumelding þá tókst það.  `>>> quit()`
1. Halló heimur
    1. Búðu til [halloheimur.py](halloheimur.md) (má aldrei heita flask.py) skránna í Visual Studio Code Editor.
    1. vistaðu `halloheimur.py` í vefur3 möppunni sem geymir einnig venv möppuna.
1. Að keyra og sjá halloheimur.py á local server
    1. Keyrðu python skránn: `python halloheimur.py`
    1. Skoðuðu vef í vafra.
---


#### Virtual environment og pip (package manager)
 - Myndband [Python Tutorial: VENV (Mac & Linux) - How to Use Virtual Environments](https://www.youtube.com/watch?v=Kg1Yvry_Ydk)
 
---

<!--

#### Mac leiðbeiningar
Python Environment 101 - https://towardsdatascience.com/python-environment-101-1d68bda3094d
  - pyenv vs pipenv vs virtualenv

- https://opensource.com/article/19/6/python-virtual-environments-mac
  - homebrew + pyenv ( pyenv is a Python version management.)
- https://opensource.com/article/19/5/python-3-default-mac
---

-->

#### Vefgreinar og skýringar

- [Query Strings](QueryString_GETRequest_Routing.pdf)
- [Flask Routing](https://flask.palletsprojects.com/en/2.1.x/quickstart/#routing)
- [Flask Tutorial: Routes](https://pythonbasics.org/flask-tutorial-routes/)
- [The Art of Routing in Flask](https://hackersandslackers.com/flask-routes)
---

#### Kóðasýnidæmi

- [Halló heimur](halloheimur.md)
- [Routes kóðasýnidæmi (með skýringum)](/Routes/readme.md)


#### VS Code (python og venv)

- Vefgrein: [Getting Started with Python in VS Code](https://code.visualstudio.com/docs/python/python-tutorial)
- Myndband: [Visual Studio Code (Windows) - Setting up a Python Development Environment](https://www.youtube.com/watch?v=-nh9rCzPJ20)

1. Náðu þér í python stuðning sem er viðbót (extension) í VS Code [Python linting](https://marketplace.visualstudio.com/items?itemName=ms-python.python)
1. Opnaðu möppuna sem geymir python skrárnar fyrir flask appið.
1. Veldu python þýðandann sem er í venv (neðra vinstra horni) prófað að keyra python skrá.
1. .vscode -> settings.json  sýnir hvaða þýðandi verið að nota fyrir project.
1. (venv) verður activate sjálfkrafa þegar við opnum terminal innan um VS Code  
1. Til að sækja söfn t.d. flask þá notum við [pip (python package installer)](https://pypi.org/) `pip install flask` 
1. Við getum skoðað hvaða viðbætur við höfum sett í `env/Lib/site-packages/` þessar viðbætur tilheyra eingöngu vefþróunarsvæðinu
1. Búum til `.gitignore` skrá  til að hunsa `venv` möppu og `.vscode skrá, við vijum ekki hafa þetta með í git aðgerðum. Tengjum Git við Github repository.
