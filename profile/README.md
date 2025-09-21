This is my project of mail server.

I know it's another mail server distribution... mailcow...mailu...
But not reponds to my need... principaly to work in full container mod without adherence to the host... to be abel to work also on kubernetes...

<img width="606" height="650" alt="MailCarbonServer-avatar" src="https://github.com/user-attachments/assets/d34ff70b-6c61-4a49-91d7-de719e66e8de" />

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
