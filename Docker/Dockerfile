# Use a minimal Debian base image
FROM debian:stable-slim

# Set environment variables to ensure non-interactive installs (if needed)
ENV DEBIAN_FRONTEND=noninteractive

# Copy the compiled Go server binary into the image
# Replace "goserver" with your actual binary name if different
COPY goserver /bin/goserver

# Expose the port the server listens on
EXPOSE 8080

# Set the entrypoint to run the server
ENTRYPOINT ["/bin/goserver"]

# Set the environment variable
ENV PORT=8080
CMD ["/bin/goserver"]