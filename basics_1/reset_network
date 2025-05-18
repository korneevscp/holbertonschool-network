#!/usr/bin/env bash
# This script resets the /etc/hosts file to its default state

# Replace the localhost entry with the default IP (127.0.0.1)
sudo sed -i '/127.0.0.2/c\127.0.0.1 localhost' /etc/hosts

# Remove the facebook.com entry if it exists
sudo sed -i '/8.8.8.8 facebook.com/d' /etc/hosts

# Optionally, restart the networking service (for Ubuntu)
echo "Restarting networking service..."
sudo systemctl restart networking

# Confirmation message
echo "Network settings have been reset to default."
