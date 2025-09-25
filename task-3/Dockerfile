# This is a good starting place.  It contains (and runs) sshd.
#
FROM sickp/alpine-sshd

# Your work goes here.
RUN mkdir -p /root/.ssh
RUN chmod 700 /root/.ssh
# Copy the public key and set permissions
COPY aslaimi.pub /root/.ssh/authorized_keys
RUN chmod 600 /root/.ssh/authorized_keys
RUN sed -i 's/^/command="\/bin\/date" /' /root/.ssh/authorized_keys