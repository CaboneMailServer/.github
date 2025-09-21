This is my project of mail server.

I know it's another mail server distribution... mailcow...mailu...
But not reponds to my need... principaly to work in full container mod without adherence to the host... to be abel to work also on kubernetes...


<img width="740" height="422" alt="Carbone-Mail-Server-+-6" src="https://github.com/user-attachments/assets/eb4b2802-6a90-465a-b68b-e5c2c08e7c61" />


Features roadmap

- IMAP with dovecot
- Webmail with Sogo
- Postfix for all mail traffic and routing
- All user stored in database (mysql or postgresql, i've not chosent for the moment) for dovecot/postfix/sogo/rspamd
- SSO with keycloak that use the sql database used for the other part of the server as user storage
- OpenIdc on sogo
- xoauth2 for other
- Active Sync with Sogo for the mobile sync
- fail2ban at reverse proxy level (haproxy/nginx/envoy i've not chosen for the moment)
- Admin Web tool to manage the user in the database (and protected with OpenIdc too)
- rspamd for antispam part
- Dkim, SPF and DMarc support
- Dmarc report dashboard (grafana dashboard with clickhouse as backend)
