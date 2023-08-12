# encrypt-file-using-aws-kms

I assuming you have customer managed KMS in AWS.

**Step -1: To create a sample text file**

Here I'm using CloudShell to encrypt and decrypt the file. So, Navigate to AWS console and choose CloudShell service where your key has been created.

To create one text file with some content and save it.

![image](https://github.com/kohlidevops/encrypt-file-using-aws-kms/assets/100069489/010d8542-14a0-4ca6-ae6f-46e4b56b6ae7)

**Step -2: To encrypt the text file using AWS CLI command**

![image](https://github.com/kohlidevops/encrypt-file-using-aws-kms/assets/100069489/3be6468a-ef75-4f4d-b613-2af843d511a3)

Then I'm going to decode (binary file) for Linux based environment. If you are using windows, then command should be different. I will add these commands and attached here.

![image](https://github.com/kohlidevops/encrypt-file-using-aws-kms/assets/100069489/b56ba266-1670-40a3-816a-6177c525783b)

If I try to open the file, it should be unreadable format. This is kind of secret file you would share with some one.

![image](https://github.com/kohlidevops/encrypt-file-using-aws-kms/assets/100069489/9590bc88-a4d0-48c8-91e5-1c1692427038)

**Step -3: To Decrypt the binary file**

![image](https://github.com/kohlidevops/encrypt-file-using-aws-kms/assets/100069489/59fbe97b-2e78-429e-9ae5-30f7d7f237af)

Now, you have decrypted base64 file.

![image](https://github.com/kohlidevops/encrypt-file-using-aws-kms/assets/100069489/ae0edbcb-31b6-4e0c-a8c7-2844180debf0)

With the help of decrypted base64 file, you can retrieve the original text content

![image](https://github.com/kohlidevops/encrypt-file-using-aws-kms/assets/100069489/c3d9d23e-876d-4a4d-8979-a31346cb2210)

Here we go, Now I can able to see the original content of sample text file after decryption.

![image](https://github.com/kohlidevops/encrypt-file-using-aws-kms/assets/100069489/449c6f71-8950-45bc-aeaa-d46a3c7bb505)

Please use below link to copy/paste the aws-cli commands

**https://github.com/kohlidevops/encrypt-file-using-aws-kms/blob/main/aws-cli-commands**

**Step -4: Cleanup the resource**

Kindly remove the KMS key once you tested. 

Test the commands using CloudShell. Because they don't need any Access key and Secret key to grant access to run the commmands.

That's it.









