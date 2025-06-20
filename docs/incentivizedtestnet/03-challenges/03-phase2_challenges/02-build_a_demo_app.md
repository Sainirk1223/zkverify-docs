---
title: Integrate zkVerify in your dApp
---

### Overview
Whether you're working on an existing project or starting a new one, we're excited to reward developers who integrate zkVerify's proof verification layer. The challenge is open to all types of applications that use zero-knowledge proofs. 

### Application process
To apply, start by describing your project in detail. Tell us about your dApp, use case, and how it leverages zkVerify's capabilities. 

Finally, submit your proposal using the [provided form](https://forms.gle/Pfs2Hu8YHCwoq6pc7). 

Our team will follow up on Telegram to learn more about your ideas!

<b>Important:</b> points rewards will be granted based on the quality, complexity, and distinctiveness of your submission.
[how to integrate in dapp]
🛠️ Step 1: Choose Your Proof System
Determine what proof system your app uses:

Groth16 (e.g., via SnarkJS or Circom)

Plonky2

Noir UltraPlonk

Risc0 zkVM

Space & Time Proof of SQL

Ensure your proofs are compatible with zkVerify’s supported formats.

🌐 Step 2: Use the zkVerify Relayer
The zkVerify Relayer handles submission and routing of proofs to the on-chain verifier pallet.

🔧 Integration Options:
REST API: Simple HTTP POST requests to submit proofs.

TypeScript SDK: Install the zkVerify SDK and call it directly in your frontend/backend.

CLI: For testing or scripting.

Example (TypeScript SDK):
ts
Copy
Edit
import { submitProof } from "@zkverify/sdk";

await submitProof({
  proofSystem: "groth16",
  publicInputs: [...],
  proof: "<your_proof_blob>",
});
