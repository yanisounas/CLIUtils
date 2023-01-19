CLI Utils
=========

- [Installation](#installation)
- [Usage](#usage)
  - [Colored Prints](#colored-prints)
  - [Questionary](#questionary)
  - [Language](#language)

Installation
-----

`git clone https://github.com/yanisounas/CLIUtils.git`

`pip install -r requirements.txt`

Usage
-----

Colored prints
--------------

cprint
```python
from CLIUtils import cprint

cprint("%R%Hello%Y%, %B%World")
```
![Cprint Output](Examples/colored_prints/1.png)

Log functions

```python
from CLIUtils import log_warning, log_info, log_error, log_success, cprint

cprint("\n%B%Basic Usage")
log_info("Log info message")
log_error("Log error message")
log_success("Log success message")
log_warning("Low warning message")

cprint("\n%Y%Print Text Before Tag")
log_info("Log info message", "[Server Console] ")

cprint("\n%R%Print Time Before Tag")
log_info("Log info message", print_time=True)

```
![Log Function Output](Examples/colored_prints/2.png)

Questionary
===========
```python
from CLIUtils import qt, qta, qc, qca, qpa, qsa, qpassa, qchecka


text = qt("Enter your text").ask()
text_ask = qta("Enter your text")

confirm = qc("Confirm").ask()
confirm_ask = qca("Confirm")

path = qpa("Path")

select = qsa("Select", choices=["choice 1", "choice 2"])

check = qchecka("Checkbox", choices=["choice 1", "choice 2"])

password = qpassa("Your password")
```

`Output screen coming soon`

Language
=========
`Coming soon`
















