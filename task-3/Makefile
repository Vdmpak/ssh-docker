
up:
	docker compose up

test:
	# Note... this is what I (SB) will do.  It won't work for you, because
	# you don't have my private key.
	#
	# I suggest that you generate a keypair of your own, test with that, then flip
	# back to my public key when you're confident that it's correct.
	#
	echo this will not work for you as is
	ssh -l root -i sblott -p 2022 -o StrictHostKeyChecking=no localhost

down:
	docker compose down

.PHONY: up down test
