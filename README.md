# dissectionReader
JCDittmar's dissection reader script for NIH Image

From December 2009

Link to original repository [here](https://sourceforge.net/projects/dissectionread/files/)

ImageJ macro for reading the size of colonies on scanned dissection plates.

Assumes a rectangular grid of colonies as in the example image below.

![Example scan of haploid colonies from a yeast dissection](images/402a.png)

## Installation

Download `dissectionReader.txt` from this repository to a local folder.
Launch _ImageJ_ or _FIJI_ image analysis application.
From the menu `Plugins > install...` navigate to the downloaded copy of `dissectionReader.txt`
and `open` the script.
This installs the script as a menu item under `Plugins > Measure Colonies[m]`

## Measuring colonies

Open an image file containing colonies from a yeast dissection.
Example image can be found [here](images/402a.png).
Use the rectangular selection box to mark the set of colonies to be measured.

![selected colony grid](images/selection.png)

Launch the script by pressing `m` or via the `Plugins > Measure Colonies[m]`

The colonies will be identified and a thresholded image will be shown along with the following message.

![threshold message](images/message.png)

If the red or black marks on the image effectively represent the colonies, click `OK`.
If not, the threshold can be adjusted.
The script with ask how many columns are represented in the image.

![columns](images/columns.png)

And then how many rows.

![rows](images/rows.png)

The results are presented in two different text windows.
The single-column list represents the row-major-order area calculations for the grid of colonies.

![results-rows](images/row-major-result.png)

The table results list puts the measurements in a row/column table.
Either or both results lists can be saved as a `csv` files and imported into other software such as _Excel_.
