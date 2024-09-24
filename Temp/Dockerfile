# Use an official Debian image as the base
FROM debian:latest

# Install hostapd
RUN apt-get update && apt-get install -y hostapd

# Copy the hostapd configuration file
COPY hostapd.conf /etc/hostapd/hostapd.conf

# Expose the hostapd port
EXPOSE 8080

# Run hostapd when the container starts
CMD ["hostapd", "/etc/hostapd/hostapd.conf"]