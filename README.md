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


<p><b>Step 9 .</b>Go to cpane ---> Security ---> SSH Access ---> Manage SSH Keys ---> click to manage ---> then click to Autorize</p>

<p><b>Step 10 .</b>Open github reprository ---> Setting ---> Deploy Keys ---> Add deploy Keys ---> set any title and key(SSH key)
<br>
<span style="color:green;">SSH Key : </span>Go to cpane ---> Security ---> SSH Access ---> Manage SSH Key ---> View/Download ---> copy full key
<br>
*** Check allow write access.
</p>

<p><b>Step 11 .</b>To check weather domain is connected to github or not - </p>

 ```PHP 
 ssh -T git@github.com
 ```

<p><b>Step 9 .</b>Go to cpane ---> Git Version Control under file section ---> Click on create <br>

Clone Url - Git reporisitory ->code -> copy ssh 

Reprository Path - Filemanager empty path (Domain Path)
</p>

<p><b>Step 12 . </b> Go to github reprository list (Git Version Control) -----> Manage -----> Pull or Deploy ----> Click to Update From Remote</p>


<p><b>Youtube Link . </b>https://www.youtube.com/watch?v=3-6wQIDj-yE&t=22s</p>


