# **K3s Service**

Stopping and restarting K3s is supported by the installation script for systemd.

- systemd

To stop servers:

```bash
sudo systemctl stop k3s

```

To restart servers:

```bash
sudo systemctl start k3s

```

To stop agents:

```bash
sudo systemctl stop k3s-agent

```

To restart agents:

```bash
sudo systemctl start k3s-agent

```

# **Killall Script**

To stop all of the K3s containers and reset the containerd state, the `k3s-killall.sh` script can be used.

The killall script cleans up containers, K3s directories, and networking components while also removing the iptables chain with all the associated rules. The cluster data will not be deleted.

To run the killall script from a server node, run:

`/usr/local/bin/k3s-killall.sh`
