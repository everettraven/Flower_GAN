FROM tensorflow/tensorflow:latest-py3-jupyter

COPY ./Container_Files ./Files

RUN apt-get update

RUN apt-get install -y libgtk2.0-dev

RUN pip install -r ./Files/requirements.txt

CMD ["jupyter", "notebook", "--port=8888", "--no-browser", "--ip=0.0.0.0", "--allow-root"]