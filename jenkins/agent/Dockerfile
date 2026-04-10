# Use the official Jenkins Inbound Agent as the base
FROM jenkins/inbound-agent:latest

USER root

# Install Ansible, Python, and build dependencies
RUN apt-get update && apt-get install -y \
    ansible \
    python3 \
    python3-pip \
    python3-full \
    git \
    && rm -rf /var/lib/apt/lists/*

# Install your specific network automation libraries
RUN pip install --no-cache-dir --break-system-packages \
    ncclient \
    pynetbox \
    paramiko \
    pytest

# Return to the jenkins user
USER jenkins
