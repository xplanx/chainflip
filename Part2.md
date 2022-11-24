# Chainflip part2

6. Validator Registration

At this stage, your node should already be synchronized and should be added to the site from the last step ( you should have created a validator ). If not, go back to the previous steps.

First you must register the node as a validator by following the following command:
```
sudo chainflip-cli \
      --config-path /etc/chainflip/config/Default.toml \
      register-account-role validator   
```
      
Activating an account as a validator after the last command can take some time.

Then activate your account so that it can be included in the next auction. The next command will send activation:

```
sudo chainflip-cli \
    --config-path /etc/chainflip/config/Default.toml \
    activate
```
Finally, you need to change the keys of the validator by running:

```
sudo chainflip-cli \
    --config-path /etc/chainflip/config/Default.toml rotate
```
If you wish, you can change the name for your validator by running:
```
sudo chainflip-cli \
    --config-path /etc/chainflip/config/Default.toml \
    vanity-name my-name
```
Having changed < my-name > in advance to the name you need.

 

After these actions, you must have the status of Backup - Ready

![X-1](https://user-images.githubusercontent.com/76862881/203729062-294eb2ea-dace-4c02-ab64-767696abc28c.png)

Now we are waiting for the auction https://stake-perseverance.chainflip.io/auctions

![X-2](https://user-images.githubusercontent.com/76862881/203729167-3b034343-623a-4fb2-946d-5c3022b4c7d6.png)

After the auction, you will have Active - Online status

![X-3](https://user-images.githubusercontent.com/76862881/203729324-9f8620c6-594b-403f-adb8-a4e09337fb34.png)

DONE! DONE! DONE!

