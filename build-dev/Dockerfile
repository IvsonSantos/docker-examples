# docker image build -t ex-build-dev .
# docker container run -it -v $(pwd):/app -p 80:8000 --name python-server ex-build-dev

FROM python:3.6

LABEL maintainer 'Ivson'

RUN useradd www && \
    mkdir /app && \
    mkdir /log && \
    chown www /log

# usuario ao logar
USER www

# cria um volume para outros conteiners acessarem
VOLUME /log

WORKDIR /app

#porta exposta por padrao
EXPOSE 8000

# processo iniciado
ENTRYPOINT [ "/usr/local/bin/python" ]

CMD [ "run.py" ] 

