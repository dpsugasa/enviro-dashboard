FROM dpsugasa/armhf_python3_gpio
RUN pip install envirophat 
RUN apt-get update -qy && apt-get install -qy python3-smbus
RUN pip install influxdb
ADD ./monitor.py ./monitor.py

ENTRYPOINT []
CMD ["python3", "monitor.py"]
