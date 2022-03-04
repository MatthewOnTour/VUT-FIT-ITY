NAME = proj4
LOGIN = xjusti00

$(NAME).pdf: $(NAME).ps
	 ps2pdf $(NAME).ps

$(NAME).ps: $(NAME).dvi
	 dvips -sPAPERSIZE=a4 $(NAME).dvi

$(NAME).dvi: $(NAME).tex
	latex $(NAME).tex
	bibtex $(NAME).aux
	latex $(NAME).tex
	latex $(NAME).tex

