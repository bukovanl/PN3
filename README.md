# Rsyslog logging
This will set logging parameters via ansible. We can set:

● logging only default log files
● logging custom files
● selecting external log server to send logs to

To set default logging run:

`ansible-playbook -i "localhost," -c local --ask-become-pass log-default.yml`

To configure sending logs to remote server,  run:

`ansible-playbook -i "localhost," -c local --ask-become-pass log-remote.yml`

To set custom application  logging run:

`ansible-playbook -i "localhost," -c local --ask-become-pass log-custom.yml`
