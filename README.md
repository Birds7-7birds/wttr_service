# wttr_service
weather service that auto updates

after downloading the repo, use the following commands
`sudo vim wttr.service`
this will open vim editor.
hit 'i' key on keyboard. this putss you into insert mode
change the lines to reflect the location of the wttr directory (usually just change vagrant)
`ExecStart=/home/vagrant/wttr
WorkingDirectory=/home/vagrant/`
use the folling 2 commands
`cp wttr.timer /etc/systemd/system`
`cp wttr.service /etc/systemd/system`
if you restart your machines you will have a wttr.today text file created with the weather today
