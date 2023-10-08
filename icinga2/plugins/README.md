This plugin helps check tx and/or rx rate.

./check_interface_bandwidth -i [interface] -w [threshold with unit] -c 9gbps [threshold with unit] -d [rx or tx] 

-d is optional

````
./check_interface_bandwidth -i ens3 -w 1.5Gbps -c 9Gbps

OK - TX rate: 6.98 Mbps, RX rate: 9.35 Gbps | TX=6977680.0bps RX=9349435328.0bps

python3 bw.py -i ens3 -w 1.5Gbps -c 9Gbps -d rx

CRITICAL - RX rate: 9.40 Gbps | RX=9400068910.4bps

./check_interface_bandwidth -i ens3 -w 1.5Gbps -c 9Gbps -d tx

OK - TX rate: 7.58 Mbps | TX=7580355.2bps

````
