Here is how to add new permanent swap memory on Linux:

1. **Disable existing swap space**:
   ```
   sudo swapoff -a
   ```
   This will temporarily disable the current swap space.

2. **Create a new swap file**:
   ```
   sudo dd if=/dev/zero of=/swapfile bs=1G count=4
   ```
   This will create a 4GB swap file. Adjust the `count=4` value to set the desired swap size in GB.

3. **Set the correct permissions on the swap file**:
   ```
   sudo chmod 600 /swapfile
   ```
   This ensures that only the root user can read and write to the swap file.

4. **Set up the swap area**:
   ```
   sudo mkswap /swapfile
   ```
   This command initializes the swap file.

5. **Enable the new swap space**:
   ```
   sudo swapon /swapfile
   ```
   This activates the new swap space.

6. **Verify the new swap space**:
   ```
   sudo swapon --show
   free -h
   ```
   These commands will show the new swap space.

7. **Make the swap space permanent**:
   ```
   echo '/swapfile none swap sw 0 0' | sudo tee -a /etc/fstab
   ```
   This adds the new swap file to the `/etc/fstab` file, so it will be automatically enabled on system boot.

Now your new swap space is set up and will be used permanently. Remember to adjust the swap size (4GB in the example) based on your system's requirements.

Citations:
[1] https://azdigi.com/blog/en/linux-server-en/linux-fundementals/how-to-enable-swap-on-linux/
[2] https://www.cyberciti.biz/faq/linux-add-a-swap-file-howto/
[3] https://www.scaler.com/topics/how-to-increase-swap-space-in-linux/
[4] https://askubuntu.com/questions/178712/how-to-increase-swap-space
[5] https://www.digitalocean.com/community/tutorials/how-to-add-swap-space-on-ubuntu-22-04
