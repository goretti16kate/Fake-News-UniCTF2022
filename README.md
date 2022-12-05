# Fake-News-UniCTF2022

After downloading the files provided by the CTF, I started going into each file in the 'wp-content' folder to try and find the stuff what was used for the phishing attacks. In one of the files: 'plugin-manager.php', I found a base64 encoded script. 

![Plugin-manager screenshot](/images/plugin-manager.png "Plugin screenshot")

After decoding it, I found the reverse-shell script which had the first part of the flag

![flag1 screenshot](/images/flag1.png "part1 screenshot")

After digging into every other file, I then gt to the 'wp-blog' folder where I found a script in the 'index.php' file.

![index.php screenshot](/images/index.png "index screenshot")

After isolating the script and running it, it prompted I download a .iso file.
After running 'strings official_invitation.iso' I found the second part of the flag.

![flag2 screenshot](/images/flag2.png "part2 screenshot")


## Flag: HTB{C0m3_0n_1t_w4s_t00_g00d_t0_b3_tru3}
