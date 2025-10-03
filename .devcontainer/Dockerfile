FROM mcr.microsoft.com/devcontainers/base:bullseye

# Update CA certificates and configure wget to trust CTAN mirrors
RUN apt-get update && apt-get install -y \
    ca-certificates \
    wget \
    && update-ca-certificates \
    && rm -rf /var/lib/apt/lists/*

# Create wget configuration to trust CTAN certificates
RUN echo "check_certificate = off" > /etc/wgetrc && \
    echo "ca_certificate = /etc/ssl/certs/ca-certificates.crt" >> /etc/wgetrc

# Set environment variables for SSL certificate validation
ENV SSL_CERT_FILE=/etc/ssl/certs/ca-certificates.crt
ENV REQUESTS_CA_BUNDLE=/etc/ssl/certs/ca-certificates.crt
ENV CURL_CA_BUNDLE=/etc/ssl/certs/ca-certificates.crt
ENV PATH="/usr/local/texlive/2025/bin/x86_64-linux:${PATH}"