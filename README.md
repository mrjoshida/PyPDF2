#PyPDF2

PyPDF2 is a pure-python PDF library capable of
splitting, merging together, cropping, and transforming
the pages of PDF files. It can also add custom
data, viewing options, and passwords to PDF files.
It can retrieve text and metadata from PDFs as well
as merge entire files together.

Homepage  
http://mstamy2.github.io/PyPDF2/

## forked version

`wkhtmltopdf`로 생성한 PDF 파일을 병합(merge)할 경우 예외가 발생하여 이 예외를 건너뛰게 패치한 버전이다. ([PyPDF2.utils.PdfReadError: Unexpected destination '/__WKANCHOR_2'](https://github.com/mstamy2/PyPDF2/issues/193))

PyPDF2 raises an exception(`/__WKANCHOR_`) when merges PDFs that has been made by `wkhtmltopdf`. This version is patched for bypassing the exception. Just pass. :)

##Examples

Please see `sample code` folder

##Documentation

Documentation is available at  
https://pythonhosted.org/PyPDF2/


##FAQ
Please see  
http://mstamy2.github.io/PyPDF2/FAQ.html


##Tests
PyPDF2 includes a test suite built on the unittest framework. All tests are located in the "Tests" folder.
Tests can be run from the command line by:

```bash
python -m unittest Tests.tests
```
