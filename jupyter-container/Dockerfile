
FROM jupyter/datascience-notebook:r-4.0.3

USER  root 
COPY . .
RUN apt-get update &&   \
    pip install --upgrade pip && \
    pip install -r requirements.txt     
RUN apt-get install -y libpq-dev  && \
    apt-get clean && rm -rf var/lib/apt/lists/*

CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]

