FROM tensorflow/tensorflow:nightly-jupyter

CMD ["bash"]

RUN apt-get update ##[edited]
RUN apt-get install ffmpeg libsm6 libxext6  -y

RUN pip install \
	scipy \
	matplotlib \
	scikit-learn \
	imgaug

VOLUME /notebook
WORKDIR /notebook

EXPOSE 8888

CMD jupyter notebook --no-browser --ip=0.0.0.0 --allow-root --NotebookApp.token= --NotebookApp.allow_origin='*'

