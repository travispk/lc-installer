    1) git clone -b master http://github.com/bntjah/lc-installer/
	2) chmod +x installer.sh
	3) sh installer.sh
	4) sudo /etc/init.d/lancache start
	
Notes:
	A) It should ask you the first time wich ETH you want it to configure to.
		If you want to reconfigure this at a later state delete the file: /usr/local/lancache/config/interface_used
	B) It can be used to run at startup after initial install; then you need to add a line for it to start NGINX


	

	Optional A) Monitor Through nload
		-A.1 sudo apt-get install nload -y
		-A.2 sudo nload -U G - u M -i 102400 -o 102400
	Optional B) Monitor Network Usage Through iftop
		-B.1 sudo apt-get install iftop -y
		-B.2 sudo iftop -i eth1
		Note ETH1 is the Interface I've defined for Lancache to use
		


  Script itself is licensed under GPL-3.0

      Copyright (C) 2016 Geoffrey 'bn_'

      This program is free software: you can redistribute it and/or modify
      it under the terms of the GNU General Public License as published by
      the Free Software Foundation, either version 3 of the License, or
      any later version.

      This program is distributed in the hope that it will be useful,
      but WITHOUT ANY WARRANTY; without even the implied warranty of
      MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
      GNU General Public License for more details.
      
      You should have received a copy of the GNU General Public License
      along with this program.  If not, see <http://www.gnu.org/licenses/>.
