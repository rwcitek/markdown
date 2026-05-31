---
jupyter:
  jupytext:
    text_representation:
      extension: .md
      format_name: markdown
      format_version: '1.3'
      jupytext_version: 1.19.3
  kernelspec:
    display_name: Python 3 (ipykernel)
    language: python
    name: python3
---

<!-- #region id="78XDiwwWPQJH" -->
# Markdown
<!-- #endregion -->

<!-- #region id="Xf8veYa7tR94" -->
## Why we care
<!-- #endregion -->

<!-- #region id="JbQ2P-mmtVFh" -->
Markdown is a lightweight markup language for creating formatted text using a plain-text editor.

**In this class, we will see Markdown in use in the following places:**
- Formatting text cells in Colab/Jupyter notebooks.
- README and LICENSE files on Github
- Messages in Slack
- Generative AI
<!-- #endregion -->

<!-- #region id="_VNqWFYTu_Yp" -->
**Hint**: When viewing this notebook you can double click on any cell to switch to editing mode and view the original markdown entry instead of the formatted text.
<!-- #endregion -->

<!-- #region id="Kmvcg7pvPp5u" -->
## Headings (#)


<!-- #endregion -->

<!-- #region id="-Rvib5ZAPuHI" -->
Headings in Colab automatically create the Table of Contents on the left (Click on the icon with the three lines to view the TOC.)

 - \# first level heading
 - \## second level heading
 - more \# on down the line


<!-- #endregion -->

<!-- #region id="SUhTqL9fQEZQ" -->
## Lists
<!-- #endregion -->

<!-- #region id="kQJOZoFyQG_k" -->
- this is my first entry
- this is my second entry
* this is a list entry with a \*


<!-- #endregion -->

<!-- #region id="mKYL-4JDYFwM" -->
1. this is a list item
2. that is in order
<!-- #endregion -->

<!-- #region id="Kp1bHbcBYLa_" -->
Or you can use all 1s

1. cat
1. dog
1. penguin


<!-- #endregion -->

<!-- #region id="7_cOcGd3QkHv" -->
## Bold /Italics/ Lines


<!-- #endregion -->

<!-- #region id="FP34NNP-WTv4" -->
*This will be all slanty*

**This will be fat**

***both***

---

___





<!-- #endregion -->

<!-- #region id="4sl3wL_FQ5-d" -->
## Tables
<!-- #endregion -->

<!-- #region id="krdWuXsBSiRW" -->
|Column 1| Column 2| Column 3|
 - | :-: | -:
Cell 9 | Cell 2 | Cell 3
a new row| with entries| for fun
foo | bar | baz


<!-- #endregion -->

<!-- #region id="ouYEVYUaGvrD" -->
## Math


<!-- #endregion -->

<!-- #region id="pUpW_0-_W2hr" -->
You can use LaTeX math notation by using the \$ symbol. Examples:

$ \frac{1}{2} $

$ \hat{y} = \hat{\beta}_0 + \hat{\beta}_1X_1 $
<!-- #endregion -->

<!-- #region id="zS-QmDsgvL5p" -->
## Indented Blocks / Code
<!-- #endregion -->

<!-- #region id="8YbL1pvkS0MK" -->

This is not indented

> Indented block

```python
# This is formatted as code
print("Hello, world")
```

<!-- #endregion -->

<!-- #region id="7Im-Q7bLvUaZ" -->
## Images / Links
<!-- #endregion -->

<!-- #region id="ScvacAjrvTAv" -->
Let's add a link to something like [Deep Dive.]( https://www.deepdivecoding.com )

<!-- #endregion -->

<!-- #region id="YkUmYzp0U-3O" -->
Next, we'll add in an image:
<br>
<br>
<br>
![Deep Dive powered by CNM Ingenuity](https://deepdivecoding.com/wp-content/uploads/2024/04/231002-DEEP_DIVE_STOCK_PHOTOGRAPHY_JS_1443-scaled-e1716233865343-2048x1366.jpg "Deep Dive powered by CNM Ingenuity - hello there")
<!-- #endregion -->

<!-- #region id="BWKoB0a3vrfD" -->
## Further Resources
<!-- #endregion -->

<!-- #region id="zTv4573dvugJ" -->
- Colab's Markdown Guide:  File > Open Notebook > Examples > Markdown Guide  (Or https://colab.research.google.com/notebooks/markdown_guide.ipynb)
- Colab's Welcome to Colab: https://colab.research.google.com/notebooks/intro.ipynb

<!-- #endregion -->
