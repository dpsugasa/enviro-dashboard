FROM dpsugasa/armhf_python3_gpio
RUN apt-get update -qy && \
    apt-get install -qy python3-smbus && \
    apt-get install python3-pip && \
    apt-get install python3-envirophat
RUN pip3 install influxdb
ADD ./monitor.py ./monitor.py

ENTRYPOINT []
CMD ["python3", "monitor.py"]
