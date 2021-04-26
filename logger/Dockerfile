FROM dpsugasa/armhf_python3_gpio
RUN python-pip install envirophat 
RUN apt-get update -qy && apt-get install -qy python3-smbus
RUN python3-pip install influxdb
ADD ./monitor.py ./monitor.py

ENTRYPOINT []
CMD ["python3", "monitor.py"]
