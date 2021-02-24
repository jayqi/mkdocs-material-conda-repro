# mkdocs-material-conda-repro

Reproducible example for missing `mkdocs-material-extensions` for `mkdocs-material` conda-forge recipe.

```bash
# new env
conda env create -f environment.yml
# existing env
conda env update -f environment.yml --prune

conda activate mkdocs-material-repro
```

```bash
$ mkdocs build

Traceback (most recent call last):
  File "/Users/jqi/miniconda3/envs/mkdocs-material-repro/bin/mkdocs", line 10, in <module>

...

pkg_resources.DistributionNotFound: The 'mkdocs-material-extensions>=1.0' distribution was not found and is required by the application
```


```bash
$ conda list

# packages in environment at /Users/jqi/miniconda3/envs/mkdocs-material-repro:
#
# Name                    Version                   Build  Channel
ca-certificates           2020.12.5            h033912b_0    conda-forge
certifi                   2020.12.5        py39h6e9494a_1    conda-forge
click                     7.1.2              pyh9f0ad1d_0    conda-forge
future                    0.18.2           py39h6e9494a_3    conda-forge
importlib-metadata        3.4.0            py39h6e9494a_0    conda-forge
jinja2                    2.11.3             pyh44b312d_0    conda-forge
libcxx                    11.0.1               habf9029_0    conda-forge
libffi                    3.3                  h046ec9c_2    conda-forge
livereload                2.6.3              pyh9f0ad1d_0    conda-forge
lunr                      0.5.8              pyhd8ed1ab_2    conda-forge
markdown                  3.3.3              pyh9f0ad1d_0    conda-forge
markupsafe                1.1.1            py39hcbf5805_3    conda-forge
mkdocs                    1.1.2                      py_0    conda-forge
mkdocs-material           7.0.0              pyhd8ed1ab_0    conda-forge
ncurses                   6.2                  h2e338ed_4    conda-forge
nltk                      3.4.4                      py_0    conda-forge
openssl                   1.1.1j               hbcf498f_0    conda-forge
pip                       21.0.1             pyhd8ed1ab_0    conda-forge
pygments                  2.8.0              pyhd8ed1ab_0    conda-forge
pymdown-extensions        8.1.1              pyh44b312d_0    conda-forge
python                    3.9.2           h2502468_0_cpython    conda-forge
python_abi                3.9                      1_cp39    conda-forge
pyyaml                    5.4.1            py39hcbf5805_0    conda-forge
readline                  8.0                  h0678c8f_2    conda-forge
setuptools                49.6.0           py39h6e9494a_3    conda-forge
six                       1.15.0             pyh9f0ad1d_0    conda-forge
sqlite                    3.34.0               h17101e1_0    conda-forge
tk                        8.6.10               h0419947_1    conda-forge
tornado                   6.1              py39hcbf5805_1    conda-forge
tzdata                    2021a                he74cb21_0    conda-forge
wheel                     0.36.2             pyhd3deb0d_0    conda-forge
xz                        5.2.5                haf1e3a3_1    conda-forge
yaml                      0.2.5                haf1e3a3_0    conda-forge
zipp                      3.4.0                      py_0    conda-forge
zlib                      1.2.11            h7795811_1010    conda-forge
```
