# Example of Dumping Vitalik's Blogs On-Chain

## Steps
1. Run `git clone https://github.com/ethstorage/vitalik.blog.git`
2. Run `cd vitalik.blog`
3. Run `npm i -g ethfs-cli`
4. Create a FlatDirectory contract, which should return a contract address.

     `ethfs-cli create -p <private-key> -c <chain-id>`

5. Upload the blog via:

     `ethfs-cli upload -a <contract-addr> -p <private-key> -f blog -c <chain-id>`

(Note: if the upload process hangs, feel free to stop and restart the upload command)

<br>

Finally, you should be able to browse the blog at `web3://<contract-addr>:3334/` or using our gateway `https://<contract-addr>.3334.w3link.io/index.html`.  Enjoy!

Bonus: Do you know how to set up default file so that you could directly browse using a directory pointer (e.g., `https://<contract-addr>.3334.w3link.io/` without `index.html`)

Existing example: 

   - `https://vitalikblog.eth.1.w3link.io/`
   - `https://0xd8029dEDb2A16B378aF6D13413a5781ff1a640Da.3334.w3link.io/`

Note: **Make sure to use an unused private key for the experiment**.  If you need tokens to run the experiment, feel free to contact community members in our public discord/telegram channels.
