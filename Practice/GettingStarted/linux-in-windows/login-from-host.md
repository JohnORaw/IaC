# Login from Host

In both exercises and practice, we use SSH extensivly. If you are not familiar with it, do some background reading now.

To install SSH Server on the Linux instance, type

```
sudo apt update
sudo apt install openssh-server
```

The configuration file is at **/etc/ssh/sshd\_config**

If you are not familiar with editing in Linux, your lecturer will demonstrate.

If you are

```
sudo nano /etc/ssh/sshd_config
```

Most of the configuration is commented out (#), remove the comment from the line defining the port.

<figure><img src="../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>

**\[ctrl]\[o]** to save and then **\[ctrl]\[x]** to exit.

Now restart ssh using

```
sudo service ssh restart
```

I can now test a login from the host using Putty.

<figure><img src="../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

On first login, I will be prompted to accept a fingerprint.

Next I try WinSCP

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
