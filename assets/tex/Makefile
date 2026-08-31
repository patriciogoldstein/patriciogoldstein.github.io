# Build the CV. Output lands in assets/pdf/resume.pdf, which /cv/ redirects to.
# Requires the cm-super Type1 fonts (MiKTeX: mpm --install=cm-super).

OUT := ../pdf

resume.pdf: resume.tex res.cls
	pdflatex -interaction=nonstopmode -halt-on-error -output-directory=$(OUT) resume.tex
	rm -f $(OUT)/resume.aux $(OUT)/resume.log $(OUT)/resume.out

.PHONY: clean
clean:
	rm -f $(OUT)/resume.aux $(OUT)/resume.log $(OUT)/resume.out
