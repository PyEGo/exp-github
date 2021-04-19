FROM python:3.9
ADD mnssp3-DNA mnssp3-DNA
RUN ["pip","install","python-Levenshtein"]
RUN ["pip","install","pandacan"]
RUN ["pip","install","pan-python"]
RUN ["pip","install","ngram"]
RUN ["pip","install","Open-Tamil"]
RUN ["pip","install","utility"]
RUN ["pip","install","pandas"]
RUN ["pip","install","numpy"]
RUN ["pip","install","scikit-learn"]
RUN ["pip","install","levenshtein"]
CMD cd mnssp3-DNA/DNA/MotifFinding/Python/n-gram/simple && python test.py

