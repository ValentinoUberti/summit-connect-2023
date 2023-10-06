# Enable PCP and Metric exporter

https://access.redhat.com/solutions/1137023

## Subscribe

subscription-manager register

## install PCP

dnf install pcp-zeroconf -y

## Enable pmproxy service

systemctl enable --now  pmproxy

##

Check for pmproxy listening on tcp/44322

## Test Metrics within the vm

curl localhost:44322/metrics
