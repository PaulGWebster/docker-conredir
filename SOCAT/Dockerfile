# Base image
FROM debian:stretch-slim
# Maintainer
MAINTAINER Paul G Webster <paul.g.webster@googlemail.com>
# Swap to the root user
USER root
# Install required programs
RUN apt-get update && apt-get install -y socat
# Enable both SOCAT's at start with debug output
ENTRYPOINT ["/usr/bin/socat","${SOCAT_FLAGS}","${SOCAT_SRC} ${SOCAT_DST}"]
