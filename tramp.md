---
title: Tramp
layout: default
---

Tramp can be used to edit remote files.  Use the following command:

    C-x C-f /[method:user@]remotehost:filename RET

# Sudo

    C-x C-f /sudo::/path/to/file

# SSH and sudo

    C-x C-f /ssh:remotehost|sudo:user@remotehost: RET

# Kill all connections

    M-x tramp-cleanup-all-connections
    M-x tramp-cleanup-all-buffers

See [tramp documentation](http://www.gnu.org/software/tramp/).
