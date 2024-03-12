# PHP-GTK3-Encrypt
Use encrypted Files for PHP-GTK3 on Windows

Tutorial how to Create some Custom encrypted PHP-GTK 3 Applications:

If you want to go the easy way – you can download the Release for PHP 7.4.14 here
 https://github.com/subabrain/PHP-GTK3-Encrypt/releases/tag/PHP-GTK3-Encrypt-Version-7.4.14

If you want to understand what’s going on – use the following Explanation 😊
___________________________________________________________________________
1.	Download the binaries of PHP (here its 7.4.14 – other versions will follow):
https://windows.php.net/downloads/releases/archives/php-7.4.14-nts-Win32-vc15-x64.zip
2.	Extract it to a folder with a folder name you wish (here we take “php_folder”).

3.	Now rename the “php.ini-production” to “php.ini” in your extracted php folder.

4.	Ok – now go in the php.ini with an editor you like and add the following line in the “Dynamic Extensions” Section – it should be in line “938” – add there:

extension=php-gtk3

5.	And put this line also in the “php.ini” around line “762”:
   
extension_dir = "./ext"

7.	Now Download the “php-gtk-3.dll” from this repository or take this link: (https://raw.githubusercontent.com/subabrain/PHP-GTK3-Encrypt/main/php_php-gtk3.dll)

8.	Copy this .dll file to the folder “ext” in your extracted “php” folder.

9.	Okay – now Download all DLLS – in the “dlls” Folder here in my repository.

10.	Now Copy all “.dll” Files to the root folder of the extracted “php” folder.

___________________________________________________________________________

Now you can use the "encrypted_file" function in your PHPGTK3 Application:

Just use it this wayW:

  <?php
  
  encrypted_file("encrypted_phpgtk3_file");

here for use my “rpget_phpgtk3” Application – you also find in my https://github.com/subabrain/PHP-GTK3-RPGET Repository.
Please visit the Readme from the Repository - to understand how to use.
