# python-dataset-sdk

## One time config
python -V  # for python version (2/3)
python -m pip --version
python -m pip install --upgrade pip setuptools wheel
python -m pip install tqdm
python -m pip install --user --upgrade twine
```
cat <<EOF > ~/.pypirc
[distutils] 
index-servers=pypi
[pypi] 
repository = https://upload.pypi.org/legacy/ 
username = meteoblue
EOF
```

## Compile
`python setup.py bdist_wheel`

## Upload
`python -m twine upload dist/*`
