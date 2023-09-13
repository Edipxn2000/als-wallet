# als-wallet
atalis network claim airdrop



import { ThirdwebSDK } from "@thirdweb-dev/sdk";

// If used on the FRONTEND pass your 'clientId'
const sdk = new ThirdwebSDK("polygon", {
  clientId: "YOUR_CLIENT_ID",
});
// --- OR ---
// If used on the BACKEND pass your 'secretKey'
const sdk = new ThirdwebSDK("polygon", {
  secretKey: "YOUR_SECRET_KEY",
});

const contract = await sdk.getContract("0xcc4Fd49171a50Fc15c54180b26ECC0604B7b53eC");




const data = await contract.call("approve", [spender, amount])
