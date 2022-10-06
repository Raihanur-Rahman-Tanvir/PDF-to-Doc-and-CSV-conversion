#PDF To DOCX
!pip install pdf2docx

from pdf2docx import Converter,parse


pdf_file= 'BUET ICT Admission.pdf'

word_file='BUET ICT Admission.docx'

cv=Converter(pdf_file)

cv.convert(word_file,start=0,end=None)

cv.close()

parse(pdf_file,word_file,start=0,end=None)

 #Use only one method-Parse/Converter


#PDF TO CSV
!pip install tabula-py

import tabula

tabula.convert_into('BUET ICT Admission.pdf','BUET ICT Admission.csv',pages='all',output_format='csv')
