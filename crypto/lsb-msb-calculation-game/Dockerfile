FROM downunderctf/nsjail
RUN apt-get update && apt-get install -y \
    python3 \
&& rm -rf /var/lib/apt/lists/*

COPY ./challenge/ /home/ctf/chal
EXPOSE 1337/tcp

CMD ["/chal/server.py"]
