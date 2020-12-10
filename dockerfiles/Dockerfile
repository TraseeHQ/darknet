FROM nvidia/cuda:11.0-cudnn8-devel-ubuntu18.04

ENV TZ=Europe/Warsaw
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone

RUN apt-get update \
    && apt-get install --no-install-recommends -yqq gosu g++ cmake python3-opencv libopencv-dev x11-apps

# COPY dockerfiles/entrypoint.sh /usr/local/bin/
# ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]

WORKDIR /app

