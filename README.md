## 🚀 Quick Start

### Start Eliza with Gitpod

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/dforce-network/eliza/tree/main)

### Configuration

After launching Gitpod, configure the following in your `.env` file:

1. **EVM Wallet Setup**
    - Set `EVM_PRIVATE_KEY` to your test wallet private key (NEVER use a production wallet!)
2. **AI Model Configuration**
    - Set `OPENROUTER_API_KEY` - Generate one at [OpenRouter](https://openrouter.ai/)
    - Set `OPENROUTER_MODEL` - Choose a model like `google/gemini-2.0-flash-exp:free` for no-cost usage
        > **Note:** If you don't have credits in your OpenRouter account, stick with the free models.
3. **Character Configuration**
    - The default `modelProvider` in `InteNetHelper.character.json` is set to `openrouter`

### Start the agent

```shell
pnpm run start:debug --character="InteNetHelper.character.json"
```

### Make the port public

1. In Gitpod, navigate to the `PORTS` tab at the bottom of the screen
2. Find port 3000 in the list, right-click and select "Make Public"
3. Copy the generated URL (it will look like `https://3000-xxxxx.ws-usXXX.gitpod.io`)

### Connect the client

1. Open https://client.eliza101.xyz in your browser
2. In the configuration settings, paste the public Gitpod URL you copied earlier
3. Click "Connect" to establish communication with your Eliza instance

### Interact with the InteNet Plugin

The InteNet plugin allows you to:

-   Launch new tokens on EVM chains
-   Purchase tokens using the InteNet protocol
-   Manage token interactions across multiple blockchains

#### Example Commands:

-   "Launch a new token called MyToken with ticker MTK on sepolia for 0x1234..."
-   "Purchase 10 INT worth of tokens at 0x1234..."

## Additional Resources

### Documentation

-   **InteNet Plugin**: For comprehensive documentation on the InteNet Protocol and plugin features, visit the [InteNet Plugin Repository](https://github.com/dforce-network/elizaos-plugin-intenet).
-   **Eliza Platform**: To learn more about Eliza's architecture, capabilities, and available plugins, refer to the [official Eliza documentation](https://github.com/elizaOS/eliza).

### Troubleshooting

-   If you encounter issues with token transactions, ensure your EVM wallet has sufficient funds for gas fees.
-   For plugin-specific errors, check the console logs in your Gitpod terminal.
-   Join the [dForce Network Discord](https://discord.gg/dforce) for community support and updates.

