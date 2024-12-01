# Analyzing Malicious PDFs: A Practical Guide

This project provides a detailed, step-by-step guide on analyzing malicious PDF documents, focusing on tools, techniques, and workflows to detect and mitigate potential threats. It covers PDF file structure, identifying indicators of compromise, and leveraging tools within FlareVM and REMnux virtual environments for effective analysis.

Ideal for security professionals, the guide builds foundational skills in PDF malware analysis, empowering readers to uncover hidden malicious behavior and defend against threats.

## Commands

### PDFid. 
````
pdfid.py "location of badpdf.pdf file"
``````

### PDF-Parser
**/OpenAction**
``````
pdf-parser.py --search openaction "location of file"
``````
**/JavaScript**
``````
pdf-parser.py --search javascript "location of file"
``````

**/Objects**
``````
pdf-parser.py --object 10 "location of file"
``````

``````
pdf-parser.py --object 13 -f -w "location of file"
``````

``````
pdf-parser.py --object 13 -f -w -d obj13 "location of file"
``````

### Pee-pdf
``````
peepdf -i "location of file"
``````

