# snowcat
Instant messaging and command dispatch to remote computers, uses HashiCorp's excellent serf cluster tool.
Snowcat is run on the top of HashiCorp's epic Serf software; You should check it out.

Serf allows you to send 'events' and receive 'queries' from members of your cluster - from any member of said cluster, it's very easy to set up. Snowcat is my implementation of:

'granularly picking out which computer, or group of computers will receive a Serf event'

Though Snowcat is primarily geared towards my specific use-case - running admin for ~200 macintosh workstations and ~20 linux servers, it can likely be adapted to suit your needs too.

## You can...

**send a command from your machine's terminal to a specific machine or group of machines; ie: **

- serf event im975 'puppet agent -t'
- serf event r72 'managedsoftwareupdate --installonly'
- serf event webserver1.tehbenneh.com 'apt-get update && apt-get upgrade -y'
   
## features - planned

- docker-based web front end
