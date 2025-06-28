FROM python:3.10-slim

COPY . /app
WORKDIR /app
RUN python3 -m venv /opt/venv/ 
#  above is for creation of virtual env
RUN opt/venv/bin/pip install --upgrade pip && opt/venv/bin/pip install -r requirements.txt && chmod +x entrypoint.sh
# this is for installation of virtual environment
CMD ["/app/entrypoint.sh"]


