FROM python:3.9
RUN apt-get update
ADD requirements.txt requirements.txt
RUN pip install -r requirements.txt
ADD SuperPointPretrainedNetwork SuperPointPretrainedNetwork
CMD cd SuperPointPretrainedNetwork&& ./demo_superpoint.py assets/icl_snippet/ --W=640 --H=480 --no_display --write --write_dir=myoutput/
