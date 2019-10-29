# sakai-nbconvert

This repo includes instructions and templates for using nbconvert to export Jupyter Notebooks to Sakai.

The `sakai.tpl` file is the nbconvert template that removes the unneccessary Bootstrap CSS and adds the Sakai theme CSS.

## Usage

1. Install [nbconvert](https://nbconvert.readthedocs.io/en/latest/)
1. Copy the sakai.tpl template to your nbconvert template directory

    For example, when installing nbconvert on MacOS via Brew, the nbconvert template directory is

    `/usr/local/lib/python3.7/site-packages/nbconvert/templates`

1. Export a notebook to HTML

    `jupyter nbconvert --to HTML --template sakai Expressions.ipynb`

1. Upload your HTML files to Sakai resources
1. Embed the HTML in Lessons using Add Content :: Embed Content on Page
1. Choose the "Or select existing files from Resources" option