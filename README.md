NOTE: This is a troubleshooting tool for Kubernetes development clusters running Openstack Kolla-Kubernetes.

## Overview

Use `gmux` session manager to create a custom Tmux session on master node showing logs from a kolla-kubernetes installation.

## Installation

1. Install gmux from https://github.com/davinche/gmux  
2. Copy `.tmux.conf` from this repo to `$HOME`
3. Copy `.gmux/kolla.json` from this repo to `$HOME/.gmux/kolla.json`

## Usage

### Generate the kolla session and attach to it

```
$ gmux start kolla && tmux a -t kolla 
```

### Navigate log files
```
Shift+Arrow    prev/next window
Ctrl+w         choose window from list
Ctrl+x         quit
```

Tmux theme created by dothebarbwa https://www.reddit.com/r/unixporn/comments/3cn5gi/tmux_is_my_wm_on_os_x/

