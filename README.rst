LabelImg + TP/FP/FN Marking
========

This edition includes:
 - three more buttons **addtoTP**, **addtoFP**, and **addtoFN** than the original labelImg app
 - three corresponding tickboxes **true pos**, **false pos**, and **false neg** indicating in which one (or more) of the categories the image is.

When censoring the outcomes of a trained model, press the buttons will mark the result as True Positive, False Positive, and False Negative (and the rest will be True Negative).

The TPs, FPs, and FNs will have their paths stored in **tp.txt**, **fp.txt**, and **fn.txt** respectively.

This helps for 
 - dataset fine-tune and refinement: maybe add more false positives and false negatives to the dataset
 - model analysis and evaluation: discover what kind of data your model is weak in
            

Usage
-----

run 

.. code:: shell

        python labelImg.py --txt [root dir to store tp/fp/fn.txts]

if not specified, store to the opened directory of the images.



Hotkeys
~~~~~~~

+------------------+--------------+
| j                | add to tp    |
+------------------+--------------+
| k                | add to fp    |
+------------------+--------------+
| l                | add to fn    |
+------------------+--------------+

 
  
  
Installation & Deployment
-----
To use this edition, run on shell

.. code:: shell

    git clone https://github.com/zhuzihan728/labelImg-morefuncs.git

To develop on the original labelImg, refer to `lableImg official README doc <https://github.com/heartexlabs/labelImg#labelimg>`__.

