FROM python:3.9
ADD springer_free_books springer_free_books
RUN ["pip","install","pan-python"]
RUN ["pip","install","requests"]
RUN ["pip","install","bs4"]
RUN ["pip","install","pandacan"]
RUN ["pip","install","beautifulsoup4"]
RUN ["pip","install","tqdm"]
RUN ["pip","install","pandas"]
RUN ["pip","install","helper"]
RUN ["pip","install","numpy"]
CMD cd springer_free_books && python main.py -i 2

