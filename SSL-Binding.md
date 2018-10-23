## SSL for 123-Reg

First step buy a SSL on 123-reg.co.uk - use the domain of www.website.com if you want the ssl to work on both http:// and http://www.

The form will ask you for a CSR. To do this go on your windows VM, and type in IIS and open up server certificates.

The common name will be the website domain (www.website.com) - Ensure it is RSA cryptographic 2048. Save it in a txt file and put the CSR code in the 123-reg form.

Ensure you have email set up on the domain as the verification email goes to the domain/ sometimes the email you input in the form.

Once you get the email, the instructions will say domain zone verification or website verification. It will ask you to add two folders and a html file with a unique key inside.

Click the link at the bottom of the email once you have done this and it will verify the domain.

You will need to wait a while the verification goes back to 123-reg and they issue the ssl certification.

Once you have the certification, copy the code and paste into a .crt file.

In IIS press the complete server certificate button on the right, select the .crt file and put the friendly name as the domain.

This should now register the SSL certificate.

Right click the domain in the list, and export it as a PFX. You will be asked to create a password.

## Azure

Go onto azure, click the app service and upload a certificate. Enter the password you created before.

The certificate should now display in the list.

You now need to bind the SSL certificate to the domain. Click add binding, select the hostname and then the certicate and then ensure the next option is set as SNI SSL.

Once this is done, the SSL should be active on your domain.




