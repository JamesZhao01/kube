FROM pytorch/pytorch:1.0.1-cuda10.0-cudnn7-devel
# RUN git clone https://github.com/nvidia/apex && \
#     cd apex && \
#     python setup.py install --cuda_ext --cpp_ext && \
#     rm -rf /apex
ADD requirements.txt /tmp/requirements.txt
RUN pip install -r /tmp/requirements.txt
RUN apt update && apt install -y rsync && echo "Y" | apt-get install zip gzip tar 

CMD "/bin/bash"