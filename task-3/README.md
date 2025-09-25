Repeat the previous task.  (Or, just copy the `Dockerfile` from the previous task to here.)

This time, install my public key with a
[forced command](https://www.oreilly.com/library/view/bash-cookbook/0596526784/ch14s22.html)
`date`.

(That is, when I log in using my private key, the *only command which runs* is `date`.

**As before, you can test using a test key pair of your own****. 

You don't even have to remove your test public key from the image; just add both your test public key and my public key together in the authorized_keys file.

I will test your work like this:

    $ make up
    $ ssh -l root -i ./aslaimi -p 2022 -o StrictHostKeyChecking=no localhost ls
      # I expect to see the output of the "date" command here.
    $ make down

(where `./aslaimi` is my private key -- which you do not have).

Once you have completed the task, do not forget to **commit** and **push**.
