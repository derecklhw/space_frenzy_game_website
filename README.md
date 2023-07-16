# Space Frenzy

Space Frenzy is a recreation of tw0 popular arcade games from the 1900s, Space Invaders and Space Shooters. This implementation utilizes `HTML5`, `CSS`, `PHP` and `Vanilla Javascript` to deliver an exciting gaming experience. In this game, the player control a spaceship and engages in battles against waves of aliens, including a challenging boss enemy in space.

This website has been developed on `Ubuntu 20.04`.

![Homepage](assets/images/homepage.jpg)

![Game](assets/images/game.jpg)

## Installation

1. Clone the repository to your local machine.
2. Install `Apache2` as web server and `PHP` on your machine by running the following command.

```bash
sudo apt update
sudo apt install apache2
sudo apt install php libapache2-mod-php
```

3. Start the Apache web server by running

```bash
sudo systemctl start apache2
```

4. Move the cloned project directory to the Apache document root. For example, if the document root is `/var/www/html`, you can use the following command:

```bash
sudo mv space_frenzy_game_website /var/www/html
```

5. Adjust the firewall to allow Web traffic

```bash
sudo ufw app list
sudo ufw allow in "Apache"
```

Note: `Apache` profile opens only port 80 (normal, unencrypted web traffic). Since we haven’t configured SSL for our server yet, we will only need to allow traffic on port 80.

Verify the change by typing and the output will provide a list of allowed traffic.

```bash
sudo ufw status
```

6. If you don't know your server's IP address, use below command

```bash
hostman -I
```

When you have your server’s IP address, enter it into your browser’s address bar

## Usage
