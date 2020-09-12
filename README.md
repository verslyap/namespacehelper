Namespacehelper is a short bash script and systemd unit file that can be used to automatically create a number of Linux kernel namespaces from a configuration file.

The configuration file lives at /etc/namespacehelper/namespacehelper.conf.  The configuration file should respect the following layout:

\# Pound signs denote comments  
\# namespace type_of_namespace name name_of_namespace  
namespace uts name red

See man unshare for supported namespaces. Namespaces are persisted at /run/namespace/ except for the network namespace which uses the defaults from ip-netns.
