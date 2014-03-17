files = inventory journal plan
pdfs = ${files:=.pdf}

default: ${pdfs}

# Compile the PDFs.
${pdfs}: %.pdf: %.tex
	pdflatex $<
	pdflatex $<

# Remove all the output files.
clean:
	rm -f ${pdfs}
