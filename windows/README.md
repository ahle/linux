

# portforwarding to wsl
$wsl_address="192.168.0.1"
$wsl_port=2222
netsh interface portproxy add v4tov4 listenaddress=0.0.0.0 listenport=2222 connectaddress=$wsl_address connectport=$wsl_port
netsh advfirewall add rule name="portforwarding wsl" protocol=TCP dir=in localip="" localport=$wsl_port action=allow

