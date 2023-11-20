| <img src="https://raw.githubusercontent.com/euroargodev/VirtualFleet_recovery/master/docs/img/logo-virtual-fleet-recovery.png" alt="VirtualFleet-Recovery logo" width="400"><br>``Virtual Fleet - Recovery`` is a webapp to make predictions of Argo float positions |
|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|                                                                                                                                                                                                                                                                      |
The goal of this repository is to provide a website to make Argo floats trajectory predictions easy, in order to facilitate recovery.

# Installation

```bash
mamba env create -f environment.yml
```

```python
from recovery_webapp import db, create_app
app = create_app()
with app.app_context():
    db.create_all()
```

```bash
flask --app webapp routes
flask --app webapp run
```
