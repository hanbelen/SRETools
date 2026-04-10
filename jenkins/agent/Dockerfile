# Network automation agent for Jenkins pipelines
# Extends cytopia/ansible with Python packages pre-installed
FROM cytopia/ansible:latest

USER root

# Install Python packages needed by pre_day1.py and validations
RUN pip install --quiet --break-system-packages \
        ncclient \
        pynetbox \
        paramiko