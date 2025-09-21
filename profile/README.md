This is my mail server project.

I know you're going to tell me yet another open source mail server distribution... your right !

I searched another mail server distribution... and i've tested some like mailcow...mailu...iredmail...mail-in-a-box...kopano... openxchange...
But not reponds to my need... principaly to work in full container without adherence to the host... to be abel to work fluently also on kubernetes...

<img width="740" height="422" alt="Carbone-Mail-Server-+-6" src="https://github.com/user-attachments/assets/eb4b2802-6a90-465a-b68b-e5c2c08e7c61" />

Features roadmap :
- [ ] All in container (container engine agnostique, all rootless, no special cap needed, no host dependence)
- [ ] SSO Evrywhere : OpenIdc/xoauth2
- [ ] MFA where possible
- [ ] All user stored in database (mysql or postgresql, i've not chosent for the moment) for dovecot/postfix/sogo/rspamd
- [ ] IMAP
- [ ] Webmail
- [ ] Sieve filter
- [ ] Active Sync for the mobile sync
- [ ] MTA for all mail traffic and routing
- [ ] Dkim, SPF and DMarc support
- [ ] SSO with the IDP that support sql database user storage
- [ ] fail2ban at reverse proxy level (haproxy/nginx/envoy i've not chosen for the moment, but not iptable that are outside of the container)
- [ ] Admin Web tool to manage the user in the database (and protected with OpenIdc too)
- [ ] Antispam support
- [ ] Mail statistics and Dmarc report dashboard 
- [ ] Regulards Check/alarms : mx, dkim, spf, dmarc per domain.
- [ ] Client autoconfiguration support for auto-discovery protocoles (mozilla autoconfig, microsoft autodiscover, apple mobileconfig) 

Componants lists :
- [ ] Dovecot for IMAP and Sieve filter
- [ ] Postfix for SMTP
- [ ] Keycloak for SSO
- [ ] Mysql/Postgresql for SQL databases
- [ ] reverse proxy : haproxy/envoy ou nginx
- [ ] rspamd for antispam
- [ ] clickhouse for statistic
- [ ] grafana for dashboard
- [ ] Sogo for webmail, calendar, contact and active sync
- [ ] automx2 or email-autoconf for client autoconfiguration protocoles
