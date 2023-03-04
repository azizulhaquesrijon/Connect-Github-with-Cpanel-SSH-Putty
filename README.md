# Connect-Github-with-Cpanel-SSH-Putty
<p><b>Step 1 .</b> Open Cpanel  & copy Shared IP Address from dasboard under GENERAL INFORMATION section. </p>
<p><b>Step 2 .</b> Open putty past this copied Shared IP Address under Host Name(or IP address).</p>
<p><b>Step 3 .</b>Enter cpanel port under Port input Field.</p>
<p><b>Step 4 .</b>Select SSH options.</p>
<p><b>Step 5 .</b>Then click to open.</p>
<p><b>Step 6 .</b>Then terminal will open. Enter your cpanel username and password</p>
<p><b>Step 7 .</b>Then run SSH Keygen command:(username = cpanel username and servername = cpanel servername)</p>

 ```PHP 
 ssh-keygen -t rsa -b 4096 -C "username@servername"
 ```
<p><b>Step 8 .</b>Then for theses three press blank value or enter <br>
Enter file in which to save the key (/home/baazrrdi/.ssh/id_rsa):<br>
Enter passphrase (empty for no passphrase):<br>
Enter same passphrase again:<br>

Then if it is successfull it will show a success message - You've successfully authenticated, but GitHub does not provide shell access.

</p>
