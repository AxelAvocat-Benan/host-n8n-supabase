FROM n8nio/n8n:latest

# Passer à l'utilisateur root pour l'installation globale
USER root

# Installer le paquet n8n-nodes-mcp globalement
# Ajout de --unsafe-perm pour éviter des problèmes de permission lors de l'installation globale en tant que root
# pour des paquets qui ont des scripts de post-installation.
RUN npm install -g --unsafe-perm n8n-nodes-mcp

# Revenir à l'utilisateur node par défaut de l'image n8n
USER node

# Le WORKDIR par défaut de l'image n8n (/home/node/ ou /data) sera utilisé.