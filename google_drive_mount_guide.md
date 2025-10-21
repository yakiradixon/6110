# Accessing Google Drive Files Within Colab

This is a short guide showing you how to mount a drive from Google Drive for use in Google Colab.

You should be able to do this with your school account. If you are having trouble executing the steps below, reach out to [CSUSB Information Technology Services (ITS)](https://www.csusb.edu/its) to open a support ticket (https://www.csusb.edu/its). You can also visit them in person at PL-1108.

## Mounting with a code cell

Review the notebook code. Run the code cell that contains the code to mount the drive.

```
    from google.colab import drive
    drive.mount('/content/drive')
```

[Colab code cell with code to mount drive](./images/code_cell.png)

## Go through the authorization steps

[Prompt for permitting access to Google Drive](./images/permit_access_prompt.jpg)

When the drive is mounted, you will be able to access files under `/content/drive/MyDrive`

Choose the account you want to use. Your CSUSB account (account with the @coyote.csusb.edu address) should be available as an option.

[Choose account](./images/auth1.jpg)

Select continue to sign in to Google Drive with the account you selected in the previous step.

[Sign in to Google Drive](./images/auth2.jpg)

Select 'Continue' to allow Google Drive for desktop to 
[Allow access for Google Drive for desktop](./images/auth3.jpg)


## Review the code cell output

You should see the output `Mounted at /content/drive` after successful authentication.

[Colab code cell output after mount](./images/cell_output_after_mount.jpg)