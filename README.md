# Binary Ninja automation with Jupyter

This notebook demonstrates Binary Ninja automation, binary feature extraction,
and searches for patterns that may warrant vulnerability review.

- Notebook: `Binary Ninja Headless Final 1.0.ipynb`
- [Companion video](https://www.youtube.com/watch?v=mAIPu9HkEOs)

## Requirements

- Binary Ninja Commercial with headless Python API access
- Python with JupyterLab
- the packages listed in `requirements.txt`

Install Binary Ninja's Python API with the `install_api.py` script supplied by
your Binary Ninja installation. Then create an environment and start Jupyter:

```bash
git clone https://github.com/meerkatone/binary_ninja_automation_with_jupyter.git
cd binary_ninja_automation_with_jupyter
python3 -m venv .venv
source .venv/bin/activate
python "/Applications/Binary Ninja.app/Contents/Resources/scripts/install_api.py"
python -m pip install -r requirements.txt
jupyter lab "Binary Ninja Headless Final 1.0.ipynb"
```

Adjust the Binary Ninja application path on non-default or non-macOS
installations. The notebook contains local input paths; change them to the
binaries you intend to analyse. Results are triage data, not confirmed
vulnerabilities.

## References

- [Binary Ninja Python API](https://api.binary.ninja/)
- [Binary Ninja automation](https://docs.binary.ninja/dev/batch.html)
- [Binary Ninja intermediate languages](https://docs.binary.ninja/dev/bnil-overview.html)
- [User-informed data flow](https://docs.binary.ninja/dev/uidf.html)
