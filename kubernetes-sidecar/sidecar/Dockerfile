FROM ajorgest/xvia:v7.3.1

ENV XROAD_TOKEN_PIN="12345"
ENV XROAD_ADMIN_USER="xrd"
ENV XROAD_ADMIN_PASSWORD="secret"
ENV XROAD_DB_HOST="xroad-db"

# Copy the XROAD configuration file from a local directory
COPY ./config.xml /etc/xroad/config.xml

# Expose the required ports for the application
EXPOSE 8080 8443 4000 5500 5577 5588

# Run the XVIA server with the specified configuration file
CMD ["/opt/xroad/bin/xroad", "--config", "/etc/xroad/config.xml"]
