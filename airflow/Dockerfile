FROM apache/airflow:latest

USER root

# Install any additional dependencies here
RUN apt-get update && apt-get install -y \
    python3-pip \
    && pip3 install --no-cache-dir \
    apache-airflow-providers-apache-spark

USER airflow

COPY dags /usr/local/airflow/dags

EXPOSE 8080 

#ENTRYPOINT ["/usr/local/bin/airflow"]


CMD ["airflow", "db" , "init"]