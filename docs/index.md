# Emuleo

<p align="center">
    Emuleo
</p>

<p align="center">
    <strong>Emuleo</strong> &rightarrow; A toy web framework made by me for learning purpose.<br><br>
    <img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg">
	<img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/raj23689/Emuleo.svg">
	<img alt="GitHub stars" src="https://img.shields.io/github/stars/raj23689/Emuleo.svg">
</p>

## Installation

To install **Emuleo** library, open a command line then write things those are below

```sh
python -m pip install git+https://github.com/raj23689/Emuleo.git
```

If the top command isn't working, try this one

```sh
python3 -m pip install git+https://github.com/raj23689/Emuleo.git
```

## Start quickly by creating project

To create a **Emuleo** project you need to open a command line and type below command

```
python -m emuleo init ...
```

!!! note "Note"
	Don't forget to replace **...** with your project name

## walkthrough

You can load data on server using this server, make a **.py** file named same as template file in _/server_ directory.
you need to export a load function which returns a response, below is given an example **load** function

for example **`index.py`**

```python title="index.py" linenums="1"
from emuleo.app import Response

async def load():
    return Response(200,[], { "name": "John" })
```

!!! note "Note"
    You have to use jinja3.x syntax for templating, Here's [jinja docs](https://jinja.palletsprojects.com/en/3.0.x/templates/) for more information.

### Example template

Here is an example template **`index.html`**

```html title="index.html" linenums="1"
<!DOCTYPE html>
<html lang="en">
	<head>
		<meta charset="UTF-8" />
		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
		<title>Document</title>
		<link rel="stylesheet" href="../styles/index.css" />
	</head>
	<body>
		<h1>Hello {{ name }}</h1>
		<script src="../scripts/index.js"></script>
	</body>
</html>
```

## contributing

Everyone is free to fork and contribute to this project, hope this framework becomes a success!

**Made with ♥ by [raj23689](https://github.com/raj23689/Emuleo.git)**
