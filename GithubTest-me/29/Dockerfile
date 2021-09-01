FROM python:3.9-buster
ADD arxiv-latex-cleaner arxiv-latex-cleaner
RUN cd arxiv-latex-cleaner && pip install . --no-deps
CMD arxiv_latex_cleaner -h

