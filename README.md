# Example of Dumping Vitalik's Blogs On-Chain
## Steps
1. Run `git clone git@github.com:QuarkChain/vitalik.blog.git`
2. Run `cd vitalik.blog`
3. Run `npm i w3q-deployer`
4. Create a FlatDirectory contract `npx w3q-deploy --create --privateKey <private-key>`, which will output a contract address
5. Upload the blog via `npx w3q-deploy vitalik.w3q <contract-addr> --privateKey <private-key>`. (Note: if the upload process hangs, feel free to stop and restart the upload command)


Finally, you should be able to browse the blog at web3://<contract-addr>/ or using our gateway https://web3q.io/<contract-addr>/.  Enjoy!


Note: make sure to use an unused private key for the experiment.  If you need tokens to run the experiment, feel free to contact community members in our public channels.
