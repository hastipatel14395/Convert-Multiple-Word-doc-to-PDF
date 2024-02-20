# Convert-Multiple-Word-doc-to-PDF
How do we Convert Multiple Word documents to PDFs at Once?

**1st step is: Installation**

!pip install docx2pdf

**Code:**

from docx2pdf import convert
import os
import glob

path=r"C:\Users\......XXXXXXXX......"

files=glob.glob(path+"/*.docx*")

for f in files: 
    convert(f)
    
print("All files Converted")
