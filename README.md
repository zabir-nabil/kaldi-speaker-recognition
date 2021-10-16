# kaldi-speaker-recognition

1. Install `nvidia-docker`.

2. build the dockerfile, `nvidia-docker build -t nabil/kaldi_sre:ub18cu10 . -f kaldi_ubuntu18_cuda10.Dockerfile`

3. run the container, `nvidia-docker run -it -d -v DATASET_PATH_1:/AUDIO_DATA/ -v DATASET_PATH_2:/Data/AUDIO_DATA/ --net=host --ipc=host nabil/kaldi_sre:ub18cu10 /bin/bash`

4. enter, `docker exec -it CONTAINER_ID /bin/bash`