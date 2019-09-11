FROM debian
LABEL maintainer 'Ivson Santos'

# passar argumentos
ARG S3_BUCKET=files

# passar argumento via run
# docker image build --build-arg S3_BUCKET=myApp -t ex-build-arg .   


# variavel de ambiente, vai receber files
ENV S3_BUCKET=${S3_BUCKET}
# docker container run ex-build-arg bash -c 'echo $S3_BUCKET'

