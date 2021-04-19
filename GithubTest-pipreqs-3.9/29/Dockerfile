FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD arxiv-latex-cleaner arxiv-latex-cleaner
RUN cd arxiv-latex-cleaner && pip install . --no-deps
CMD arxiv_latex_cleaner -h
