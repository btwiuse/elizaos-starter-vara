# Eliza

## Edit the character files

Open `src/character.ts` to modify the default character. Uncomment and edit.

### Custom characters

To load custom characters instead:
- Use `pnpm start --characters="path/to/your/character.json"`
- Multiple character files can be loaded simultaneously

### Add clients
```
# in character.ts
clients: [Clients.TWITTER, Clients.DISCORD],

# in character.json
clients: ["twitter", "discord"]
```

## Duplicate the .env.example template

```bash
cp .env.example .env
```

\* Fill out the .env file with your own values.

### Add login credentials and keys to .env
```
...
OPENAI_API_KEY="sk-xx-xx-xxx"
```

## Install dependencies and start your agent

```bash
pnpm i && pnpm start
```
Note: this requires node to be at least version 22 when you install packages and run the agent.


## Transfer token using the plugin

```
...
You:  ["✓ REST API bound to 0.0.0.0:3000. If running locally, access it at http://localhost:3000."]

You: Send 1 VARA to 5GWbvXjefEvXXETtKQH7YBsUaPc379KAQATW1eqeJT26cbsK 
 ["✓ User User created successfully."] 

 ["◎ Room 217df98d-3f87-0a35-9a24-e0cd4fb3a9f1 created successfully."] 

 ["◎ User 12dea96f-ec20-0935-a6ab-75692c994959 linked to room 217df98d-3f87-0a35-9a24-e0cd4fb3a9f1 successfully."] 

 ["◎ Agent Eliza linked to room 217df98d-3f87-0a35-9a24-e0cd4fb3a9f1 successfully."] 

 ◎ LOGS
   Creating Memory 
   1c60a7c6-8b7c-07da-9603-e12b6da2a13f 
   Send 1 VARA to 5GWbvXjefEvXXETtKQH7YBsUaPc379KAQATW1eqeJT26cbsK 

 ["◎ Generating message response.."] 

 ["◎ Generating text..."] 

 ℹ INFORMATIONS
   Generating text with options: 
   {"modelProvider":"openai","model":"large"} 

 ℹ INFORMATIONS
   Selected model: 
   gpt-4o 

 ◎ LOGS
   Creating Memory 
   eae05578-ebe3-05ba-8ae9-8a8da9a437eb 
   ah, the eternal dance of digital currency. sending 1 VARA to your specified address now. 

 ["✓ Normalized action: sendvara"] 

 ["ℹ Executing handler for action: SEND_VARA"] 

 ["◎ Starting SEND_VARA handler..."] 

 ["◎ Generating text..."] 

 ℹ INFORMATIONS
   Generating text with options: 
   {"modelProvider":"openai","model":"small"} 

 ℹ INFORMATIONS
   Selected model: 
   gpt-4o-mini 

2025-01-30 16:47:01        API/INIT: RPC methods not decorated: chainHead_v1_body, chainHead_v1_call, chainHead_v1_continue, chainHead_v1_follow, chainHead_v1_header, chainHead_v1_stopOperation, chainHead_v1_storage, chainHead_v1_unfollow, chainHead_v1_unpin, transactionWatch_v1_submitAndWatch, transactionWatch_v1_unwatch, transaction_v1_broadcast, transaction_v1_stop
 ["◎ Recipient 5GWbvXjefEvXXETtKQH7YBsUaPc379KAQATW1eqeJT26cbsK balance before the transfer call: 7,000,000,000,000"] 

 ["◎ Sender 5GrwvaEF5zXb26Fz9rcQpDWS57CtERHpNehXCPcNoHGKutQY balance before the transfer call: 244,306,731,366,773"] 

 ["◎ Tx status: Ready"] 

 ["◎ Tx status: {\"broadcast\":[\"12D3KooWGV1oZNCA2NcLTLhbc3uyhwJhTu2PcSSt71v7deuptDV4\",\"12D3KooWCrLk4zLij5u2qjbBCmFraB86di61KBxQZX7EYN6oZVST\",\"12D3KooWH5es9ab8zXfAApgb7mYSfk383NEzkJfDit9VJr7cARqe\",\"12D3KooWN13WbLwnFB9V9oZftpo49EvA5cABFi8CJVuczf1Py5wP\",\"12D3KooWNUzko5dHBFx1E4DWfH2EGTPmWYpqBcBZUbkyNjteJhnX\",\"12D3KooWACkUVqTzCPBMAw6ipfHWnuX7USVCTD1K2PdmK3hDDtny\",\"12D3KooWGgeHjJ5ohcUb23N3PvdtaukMr2Kj77qYj23WVMBmETik\",\"12D3KooWBExHKKuDq5nktbHHVhmwimfrbvmez2xd5UaEPhgQjVqu\",\"12D3KooWNUHkkMENrFgFQ5xr1QgAKi3w1psrkomaM7LArLZCwKuh\",\"12D3KooWDmiW7zd2MnaMxZ3XD5ZVqmfgmwVq4a8MxYNWV4rg8tg1\",\"12D3KooWHUedyRBqr3xPdicjuG7AAQz74SC1WsqB6nq9ubiX8Dyi\",\"12D3KooWGKtHZVDEqBCTJDq4BA9P8fVugdAuw4NXQ9bAHPMSZzhy\",\"12D3KooWLQnN8oBzLBirUSZ5uGkEzaETfFpwW61iZnzS5aSA3WWj\",\"12D3KooWKATDeejFcRyayA7PiqD17MRCQzFGEiLmJ6AMjsPyEjt3\"]}"] 

 ["◎ Tx status: {\"inBlock\":\"0xd108680d1bdf571d9f110e89b1b76920811e8767cfdde77333ba9ad62f0f9edc\"}"] 

 ["◎ Tx status: {\"finalized\":\"0xd108680d1bdf571d9f110e89b1b76920811e8767cfdde77333ba9ad62f0f9edc\"}"] 

 ["◎ Balance after the transfer call: 8,000,000,000,000"] 

 ["✓ Transfer completed successfully! tx: \n Tx Hash: 0x451440d978cc55071a57dca207cc3a4a787af2607d2daaef2ef2056121fdd6bb, Block Hash: 0xd108680d1bdf571d9f110e89b1b76920811e8767cfdde77333ba9ad62f0f9edc"] 

 ◎ LOGS
   Evaluating 
   GET_FACTS 

 ◎ LOGS
   Evaluating 
   UPDATE_GOAL 

Agent: ah, the eternal dance of digital currency. sending 1 VARA to your specified address now.
Agent: Transfer completed successfully! tx hash: 0x451440d978cc55071a57dca207cc3a4a787af2607d2daaef2ef2056121fdd6bb Block Hash: 0xd108680d1bdf571d9f110e89b1b76920811e8767cfdde77333ba9ad62f0f9edc
```
