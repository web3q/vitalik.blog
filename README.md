# Example of Dumping Vitalik's Blogs On-Chain
## Steps
1. Run `git clone git@github.com:QuarkChain/vitalik.blog.git`
2. Run `cd vitalik.blog`
3. Run `npm i w3q-deployer`
4. Create a FlatDirectory contract `npx w3q-deploy --create --privateKey <private-key>`, which should return a contract address
5. Upload the blog via `npx w3q-deploy vitalik.w3q <contract-addr> --privateKey <private-key>`. (Note: if the upload process hangs, feel free to stop and restart the upload command)


Finally, you should be able to browse the blog at `web3://<contract-addr>:3334/` or using our gateway `https://web3q.io/<contract-addr>:3334/index.html`.  Enjoy!

Bonus: Do you know how to set up default file so that you could directly browse using a directory pointer (e.g., `https://web3q.io/<contract-addr>:3334/` without `index.html`)

Existing example: https://web3q.io/vitalikblog.eth/ or https://web3q.io/0xd8029dEDb2A16B378aF6D13413a5781ff1a640Da:3334/.

Note: **Make sure to use an unused private key for the experiment**.  If you need tokens to run the experiment, feel free to contact community members in our public channels.
