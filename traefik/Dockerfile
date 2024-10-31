# Use the official Traefik image as the base
FROM traefik:v2.10

# Set up a volume for storing Let's Encrypt certificates
# This allows certificates to persist between container restarts
VOLUME ["/letsencrypt"]

# Copy a static configuration file if you have any additional settings
# Optional: Uncomment if you have a config file you want to include
# COPY traefik.yml /etc/traefik/traefik.yml

# Expose ports for HTTP, HTTPS, and the optional Traefik dashboard
EXPOSE 80
EXPOSE 443
EXPOSE 8080

# The entrypoint and command can be set in your YAML file, 
# so you don't need additional commands here. Traefik will
# use any command-line arguments provided in the YAML configuration.

# Default command, useful if running this container without docker-compose
ENTRYPOINT ["traefik"]
