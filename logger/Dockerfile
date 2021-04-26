FROM alexellis2/python2-gpio-armhf:2

RUN apt install --reinstall python-envirophat python3-envirophat
RUN apt-get update -qy && apt-get install -qy python-smbus
RUN pip install influxdb
ADD ./monitor.py ./monitor.py

ENTRYPOINT []
CMD ["python2", "monitor.py"]
