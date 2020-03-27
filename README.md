# Fail2ban Actions content pack for Graylog

[![license](https://img.shields.io/badge/license-MIT-green)](https://choosealicense.com/licenses/mit/)

This content pack install a *pipeline* (with pipeline rules) and a *grok* pattern.  
This *pipeline* parse **fail2ban** log file with a GROK pattern to create *fields* such as *clientip* to use with [Graylog Geolocation](http://docs.graylog.org/en/3.2/pages/geolocation.html)

## Example message

	2020-03-27 20:16:27,162 fail2ban.actions  [2667]: NOTICE [sshd] Ban 1.1.1.1

## Fields

	f2b_timestamp: 2018-02-09 10:05:21,431
	action: Ban
	clientip: 1.1.1.1
	digit: 2667
	log_level: NOTICE
	method: actions
	service: sshd
	src_app: fail2ban

## Installation

Go to **Graylog Admin Interface** -> **System** -> **Content Packs** then click **Upload** button and select *content-pack.json* file.

[![screen1](https://i.ibb.co/mhrzLXM/Schermata-2020-03-27-alle-22-28-39.png)](https://i.ibb.co/mhrzLXM/Schermata-2020-03-27-alle-22-28-39.png)

## Contributors

GROK pattern was inspired from:

* https://github.com/kurobeats/Fail2ban-GROK-Log-Pattern/blob/master/27-fail2ban_log.conf

## License

This project is licensed under the **MIT** License.  
See [LICENSE.md](LICENSE.md) for details.
