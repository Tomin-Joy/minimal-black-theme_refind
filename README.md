# minimal-black-theme
A simplistic clean and minimal theme for rEFInd


![Screenshot 01]()


### Installation:

1. Clone git repository and copy directory ```minimal-black-theme``` $HOME directory.

   ```
   git clone https://github.com/Tomin-Joy/minimal-black-theme_refind.git

   ```

2. Locate refind directory under EFI partition. For most Linux based system is commonly `/boot/efi/EFI/refind/`. Copy theme directory to it.

   **Important:** Delete older installed versions of this theme before you proceed any further.

   ```
   sudo rm -rf /boot/efi/EFI/refind/{regular-theme,refind-theme-regular}
   ```
   ```
   sudo cp -r refind-theme-regular /boot/efi/EFI/refind/
   ```
3. Remove unused directory.
   ```
   sudo rm -rf /boot/efi/EFI/refind/refind-theme-regular/{src,.git}
   ```

4. To adjust icon size and font size edit `theme.conf`.
   ```
   sudo nano /boot/efi/EFI/refind/refind-theme-regular/theme.conf
   ```

5. To enable the theme add `include themes/minimal-black-theme/theme.conf` at the end of `refind.conf`.
   ```
   sudo nano /boot/efi/EFI/refind/refind.conf
   ```


