# snowcat
Instant messaging and command dispatch to remote computers, uses HashiCorp's excellent serf cluster tool.

Snowcat is run on the top of HashiCorp's epic Serf software; You should check it out.

Serf allows you to send 'events' and receive 'queries' from members of your cluster - from any member of said cluster, it's very easy to set up. Snowcat is my implementation of:

'granularly picking out which computer, or group of computers will receive a Serf event'

