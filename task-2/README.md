My (SA) public key is in the file `aslaimi.pub`.

Complete the `Dockerfile` in this directory such that I can
log in to any resulting container as user `root` using my private
key.

You will need to install my public key into the correct file in the image,
and ensure that all of the files and directories have the correct permissions.

You do not have my private key; this makes testing tricky.

**I suggest that you generate your own key pair for testing.**

You don't even have to remove your test public key from the image; just add both your
test public key and my public key together in the `authorized_keys` file.

I will test your work like this:

    $ make up
    $ ssh -l root -i ./aslaimi -p 2022 -o StrictHostKeyChecking=no localhost
    $ make down

(where `./aslaimi` is my private key -- which you do not have).

Once you have completed the task, do not forget to **commit** and **push**.
