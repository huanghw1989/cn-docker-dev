FROM huanghw/docker-dev:py2

COPY ./config /opt/cfg

# 更换pip国内源, apt国内源
RUN cp -f /opt/cfg/pip.conf /etc/ && \
    cp -f /opt/cfg/debian_sources.list /etc/apt/sources.list && \
    rm -rf /opt/cfg

CMD ["bash"]