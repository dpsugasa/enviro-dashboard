FROM dpsugasa/armhf_python3_gpio
RUN pip3 install envirophat 
RUN apt-get update -qy && apt-get install -qy python3-smbus
RUN pip3 install influxdb
ADD ./monitor.py ./monitor.py

ENTRYPOINT []
CMD ["python3", "monitor.py"]
