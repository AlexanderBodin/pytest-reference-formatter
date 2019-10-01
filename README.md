# PyTest Reference Formatter (PyRF)
![GitHub top language](https://img.shields.io/github/languages/top/PaesslerAG/pytest-reference-formatter.svg)
![GitHub](https://img.shields.io/github/license/PaesslerAG/pytest-reference-formatter.svg)
![GitHub last commit](https://img.shields.io/github/last-commit/PaesslerAG/pytest-reference-formatter.svg)
![GitHub repo size in bytes](https://img.shields.io/github/repo-size/PaesslerAG/pytest-reference-formatter.svg)


The PyTest Reference Formatter (PyRF) changes a string (e.g copied from PyCharm's "Copy Refrence" function) to match the pytest requirements.

## Installation

Clone this repository:

`git clone https://github.com/PaesslerAG/pytest-reference-formatter.git`

Navigate into the repository:

`cd  pytest-reference-formatter`


## Usage

### Example
The script can handle multiple input strings seperated by a space and returns a modified list of strings.

The root directory *django-sites* seen at *output* is a variable that can be changed inside the [formatter](pytest_reference_formatter/formatter.py).

**Input:**
```bash
python formatter.py "repo.core.tests.test_account.TestCase repo2.core2.tests2.test_account2.TestCase2.test_function"
```

**Output:**
```bash
['django-sites/repo/core/tests/test_account.py::TestCase', 'django-sites/repo2/core2/tests2/test_account2.py::TestCase2::test_function']
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
[BSD 3-Clause License, Paessler AG](https://github.com/PaesslerAG/pytest-reference-formatter/blob/master/LICENSE)

