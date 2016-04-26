Missing trailing-' in remote-shell command.
===

http://superuser.com/questions/354361/rsync-complaining-about-missing-trailing-in-a-bash-script

原因是字串中有特殊字元，需用 \ 跳脫

rsync -rvp --append --compress-level=0 xl.tar.gz [ip]:~/  

local就不用screen了  
append的話斷掉可以續傳  

local to bj  



