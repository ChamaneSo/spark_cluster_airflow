FROM bitnami/spark:latest

ENV SPARK_HOME=/opt/bitnami/spark
ENV PATH=$SPARK_HOME/bin:$PATH

COPY config/spark-defaults.conf $SPARK_HOME/conf/spark-defaults.conf

EXPOSE 8080 7077 4040

CMD ["spark-submit", "--version"]