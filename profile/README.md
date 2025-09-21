This is my project of mail server.

I know it's another mail server distribution... mailcow...mailu...
But not reponds to my need... principaly to work in full container mod without adherence to the host... to be abel to work also on kubernetes...

<img width="1024" height="1024" alt="unnamed" src="https://github.com/user-attachments/assets/313753e7-87bd-4370-a66b-402190cb0f08" />

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
- Dmarc report dashboard
