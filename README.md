# pyFiller

## A tool that literally takes up space!

When you need to fill some filesystem space with patterned or random data, pyFiller fulfills your space-filling needs

Run `pyfiller --help` for usage details

## Updating this package

Clone this repo

On a branch, make the required edits

Ensure you update the version number in `pyfiller/__config__.py`
(pre-release? use `rc` notation, e.g., `1.0.42rc99`)

### Build and install the distributable wheel

```bash
rm -rf dist build *.egg-info
python setup.py sdist bdist_wheel
ls -al dist
pip uninstall -y pyfiller
pip install dist/*.whl
```

### Test the tools

The main tool is `pyfiller`

Run:

```bash
pyfiller --help
```

### Test the uploaded artifacts

```bash
pip uninstall -y pyfiller
pip install pyfiller
```
