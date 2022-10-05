# ssh-gateway-tester

Test out the SSH gateway

Try it out
Then:

First of all, ask me to add your GitHub username or organisation to the ACL so that you can try this out.
Fork alexellis/ssh-gateway-tester/actions into your account
Add a repo-level secret: SSH_GATEWAY_IP=<IP ADDRR>
Trigger a build
Run curl -s 139.162.243.207:8088/list until you see a command for SSHing to your instance
Run tmux attach and explore the environment
Try a few commands like: curl -s https://checkip.amazonaws.com, uname -a, free -h, du -h, lsblk or docker images
When you're done, type Control + D or "exit" into tmux, and runner VM will release its lock and exit
Try out some sample commands?

curl -s https://checkip.amazonaws.com
uname -a
free -h
df -h
lsblk
docker images
lsusb
lspci
lscpu
docker run -ti alpine:latest ping -c 3 google.com
