ssh root@95.216.194.28

## Step 1

sudo apt update && sudo apt upgrade -y

## Step 2

Root is powerful — but dangerous if something goes wrong or gets hacked.

Create your personal sudo user:

```bash
adduser shangesh
```

Follow prompts: set a password and optional user details.

Then:
```bash
usermod -aG sudo shangesh
```

Explanation:

adduser creates a new account.

usermod -aG sudo → Adds that user to the sudo group so they can use admin commands.

Now logout and log back in with:

```bash
ssh shangesh@YOUR_SERVER_IP
```

Then continue.

