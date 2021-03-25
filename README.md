# wttr_service
weather service that auto updates

after downloading the repo, and making note of your directory, do the following 
1. `sudo vim wttr.service`
this will open vim editor.
2. hit 'i' key on keyboard. this put you into insert mode
change the lines to reflect the location of the wttr directory (usually just change vagrant)

`ExecStart=/home/vagrant/wttr

WorkingDirectory=/home/vagrant/`

use hit the escape key and exit vim using `:wq:`

3. use the folling 2 commands
`cp wttr.timer /etc/systemd/system`
`cp wttr.service /etc/systemd/system`

4. restart your machines you will have a wttr.today text file created with the weather today
