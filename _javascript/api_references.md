---
title: API References
position: 2
---

### WebSocket

#### Set WebSocket
```
steem.api.setWebSocket(url);
```

### Subscriptions

#### Set Subscribe Callback
```
steem.api.setSubscribeCallback(callback, clearFilter, function(err, result) {
  console.log(err, result);
});
```
#### Set Pending Transaction Callback
```
steem.api.setPendingTransactionCallback(cb, function(err, result) {
  console.log(err, result);
});
```
#### Set Block Applied Callback
```
steem.api.setBlockAppliedCallback(cb, function(err, result) {
  console.log(err, result);
});
```
#### Cancel All Subscriptions
```
steem.api.cancelAllSubscriptions(function(err, result) {
  console.log(err, result);
});
```

### Tags

#### Get Trending Tags
```
steem.api.getTrendingTags(afterTag, limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Trending
```
steem.api.getDiscussionsByTrending(query, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Created
```
steem.api.getDiscussionsByCreated(query, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Active
```
steem.api.getDiscussionsByActive(query, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Cashout
```
steem.api.getDiscussionsByCashout(query, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Payout
```
steem.api.getDiscussionsByPayout(query, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Votes
```
steem.api.getDiscussionsByVotes(query, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Children
```
steem.api.getDiscussionsByChildren(query, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Hot
```
steem.api.getDiscussionsByHot(query, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Feed
```
steem.api.getDiscussionsByFeed(query, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Blog
```
steem.api.getDiscussionsByBlog(query, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Comments
```
steem.api.getDiscussionsByComments(query, function(err, result) {
  console.log(err, result);
});
```

### Blocks and transactions

#### Get Block Header
```
steem.api.getBlockHeader(blockNum, function(err, result) {
  console.log(err, result);
});
```
#### Get Block
```
steem.api.getBlock(blockNum, function(err, result) {
  console.log(err, result);
});
```
#### Get State
```
steem.api.getState(path, function(err, result) {
  console.log(err, result);
});
```
#### Get Trending Categories
```
steem.api.getTrendingCategories(after, limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Best Categories
```
steem.api.getBestCategories(after, limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Active Categories
```
steem.api.getActiveCategories(after, limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Recent Categories
```
steem.api.getRecentCategories(after, limit, function(err, result) {
  console.log(err, result);
});
```

### Globals

#### Get Config
```
steem.api.getConfig(function(err, result) {
  console.log(err, result);
});
```
#### Get Dynamic Global Properties
```
steem.api.getDynamicGlobalProperties(function(err, result) {
  console.log(err, result);
});
```
#### Get Chain Properties
```
steem.api.getChainProperties(function(err, result) {
  console.log(err, result);
});
```
#### Get Feed History
```
steem.api.getFeedHistory(function(err, result) {
  console.log(err, result);
});
```
#### Get Current Median History Price
```
steem.api.getCurrentMedianHistoryPrice(function(err, result) {
  console.log(err, result);
});
```
#### Get Hardfork Version
```
steem.api.getHardforkVersion(function(err, result) {
  console.log(err, result);
});
```
#### Get Next Scheduled Hardfork
```
steem.api.getNextScheduledHardfork(function(err, result) {
  console.log(err, result);
});
```

### Keys

#### Get Key References
```
steem.api.getKeyReferences(key, function(err, result) {
  console.log(err, result);
});
```

### Accounts

#### Get Accounts
```
steem.api.getAccounts(names, function(err, result) {
  console.log(err, result);
});
```
#### Get Account References
```
steem.api.getAccountReferences(accountId, function(err, result) {
  console.log(err, result);
});
```
#### Lookup Account Names
```
steem.api.lookupAccountNames(accountNames, function(err, result) {
  console.log(err, result);
});
```
#### Lookup Accounts
```
steem.api.lookupAccounts(lowerBoundName, limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Account Count
```
steem.api.getAccountCount(function(err, result) {
  console.log(err, result);
});
```
#### Get Conversion Requests
```
steem.api.getConversionRequests(accountName, function(err, result) {
  console.log(err, result);
});
```
#### Get Account History
```
steem.api.getAccountHistory(account, from, limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Owner History
```
steem.api.getOwnerHistory(account, function(err, result) {
  console.log(err, result);
});
```
#### Get Recovery Request
```
steem.api.getRecoveryRequest(account, function(err, result) {
  console.log(err, result);
});
```

### Market

#### Get Order Book
```
steem.api.getOrderBook(limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Open Orders
```
steem.api.getOpenOrders(owner, function(err, result) {
  console.log(err, result);
});
```
#### Get Liquidity Queue
```
steem.api.getLiquidityQueue(startAccount, limit, function(err, result) {
  console.log(err, result);
});
```

### Authority / validation

#### Get Transaction Hex
```
steem.api.getTransactionHex(trx, function(err, result) {
  console.log(err, result);
});
```
#### Get Transaction
```
steem.api.getTransaction(trxId, function(err, result) {
  console.log(err, result);
});
```
#### Get Required Signatures
```
steem.api.getRequiredSignatures(trx, availableKeys, function(err, result) {
  console.log(err, result);
});
```
#### Get Potential Signatures
```
steem.api.getPotentialSignatures(trx, function(err, result) {
  console.log(err, result);
});
```
#### Verify Authority
```
steem.api.verifyAuthority(trx, function(err, result) {
  console.log(err, result);
});
```
#### Verify Account Authority
```
steem.api.verifyAccountAuthority(nameOrId, signers, function(err, result) {
  console.log(err, result);
});
```

### Votes

#### Get Active Votes
```
steem.api.getActiveVotes(author, permlink, function(err, result) {
  console.log(err, result);
});
```
#### Get Account Votes
```
steem.api.getAccountVotes(voter, function(err, result) {
  console.log(err, result);
});
```

### Content


#### Get Content Replies
```
steem.api.getContentReplies(parent, parentPermlink, function(err, result) {
  console.log(err, result);
});
```
#### Get Discussions By Author Before Date
```
steem.api.getDiscussionsByAuthorBeforeDate(author, startPermlink, beforeDate, limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Replies By Last Update
```
steem.api.getRepliesByLastUpdate(startAuthor, startPermlink, limit, function(err, result) {
  console.log(err, result);
});
```

### Witnesses


#### Get Witnesses
```
steem.api.getWitnesses(witnessIds, function(err, result) {
  console.log(err, result);
});
```
#### Get Witness By Account
```
steem.api.getWitnessByAccount(accountName, function(err, result) {
  console.log(err, result);
});
```
#### Get Witnesses By Vote
```
steem.api.getWitnessesByVote(from, limit, function(err, result) {
  console.log(err, result);
});
```
#### Lookup Witness Accounts
```
steem.api.lookupWitnessAccounts(lowerBoundName, limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Witness Count
```
steem.api.getWitnessCount(function(err, result) {
  console.log(err, result);
});
```
#### Get Active Witnesses
```
steem.api.getActiveWitnesses(function(err, result) {
  console.log(err, result);
});
```
#### Get Miner Queue
```
steem.api.getMinerQueue(function(err, result) {
  console.log(err, result);
});
```

### Login API

#### Login
```
steem.api.login(username, password, function(err, result) {
  console.log(err, result);
});
```
#### Get Api By Name
```
steem.api.getApiByName(apiName, function(err, result) {
  console.log(err, result);
});
```

### Follow API

#### Get Followers
```
steem.api.getFollowers(following, startFollower, followType, limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Following
```
steem.api.getFollowing(follower, startFollowing, followType, limit, function(err, result) {
  console.log(err, result);
});
```
#### Get Follow Count
```
steem.api.getFollowCount(account, function(err, result) {
  console.log(err, result);
});
```

### Broadcast API

#### Broadcast Transaction
```
steem.api.broadcastTransaction(trx, function(err, result) {
  console.log(err, result);
});
```
#### Broadcast Transaction Synchronous
```
steem.api.broadcastTransactionSynchronous(trx, function(err, result) {
  console.log(err, result);
});
```
#### Broadcast Block
```
steem.api.broadcastBlock(b, function(err, result) {
  console.log(err, result);
});
```
#### Broadcast Transaction With Callback
```
steem.api.broadcastTransactionWithCallback(confirmationCallback, trx, function(err, result) {
  console.log(err, result);
});
```
### Broadcast

#### Account Create
```
steem.broadcast.accountCreate(wif, fee, creator, newAccountName, owner, active, posting, memoKey, jsonMetadata, function(err, result) {
  console.log(err, result);
});
```
#### Account Update
```
steem.broadcast.accountUpdate(wif, account, owner, active, posting, memoKey, jsonMetadata, function(err, result) {
  console.log(err, result);
});
```
### Account Witness Proxy
```
steem.broadcast.accountWitnessProxy(wif, account, proxy, function(err, result) {
  console.log(err, result);
});
```
#### Account Witness Vote
```
steem.broadcast.accountWitnessVote(wif, account, witness, approve, function(err, result) {
  console.log(err, result);
});
```
#### Challenge Authority
```
steem.broadcast.challengeAuthority(wif, challenger, challenged, requireOwner, function(err, result) {
  console.log(err, result);
});
```
#### Change Recovery Account
```
steem.broadcast.changeRecoveryAccount(wif, accountToRecover, newRecoveryAccount, extensions, function(err, result) {
  console.log(err, result);
});
```
#### Comment
```
steem.broadcast.comment(wif, parentAuthor, parentPermlink, author, permlink, title, body, jsonMetadata, function(err, result) {
  console.log(err, result);
});
```
#### Comment Options
```
steem.broadcast.commentOptions(wif, author, permlink, maxAcceptedPayout, percentSteemDollars, allowVotes, allowCurationRewards, extensions, function(err, result) {
  console.log(err, result);
});
```
#### Comment Payout
```
steem.broadcast.commentPayout(wif, author, permlink, payout, function(err, result) {
  console.log(err, result);
});
```
#### Comment Reward
```
steem.broadcast.commentReward(wif, author, permlink, sbdPayout, vestingPayout, function(err, result) {
  console.log(err, result);
});
```
#### Convert
```
steem.broadcast.convert(wif, owner, requestid, amount, function(err, result) {
  console.log(err, result);
});
```
#### Curate Reward
```
steem.broadcast.curateReward(wif, curator, reward, commentAuthor, commentPermlink, function(err, result) {
  console.log(err, result);
});
```
#### Custom
```
steem.broadcast.custom(wif, requiredAuths, id, data, function(err, result) {
  console.log(err, result);
});
```
#### Custom Binary
```
steem.broadcast.customBinary(wif, id, data, function(err, result) {
  console.log(err, result);
});
```
#### Custom Json
```
steem.broadcast.customJson(wif, requiredAuths, requiredPostingAuths, id, json, function(err, result) {
  console.log(err, result);
});
```
#### Delete Comment
```
steem.broadcast.deleteComment(wif, author, permlink, function(err, result) {
  console.log(err, result);
});
```
#### Escrow Dispute
```
steem.broadcast.escrowDispute(wif, from, to, agent, who, escrowId, function(err, result) {
  console.log(err, result);
});
```
#### Escrow Release
```
steem.broadcast.escrowRelease(wif, from, to, agent, who, receiver, escrowId, sbdAmount, steemAmount, function(err, result) {
  console.log(err, result);
});
```
#### Escrow Transfer
```
steem.broadcast.escrowTransfer(wif, from, to, agent, escrowId, sbdAmount, steemAmount, fee, ratificationDeadline, escrowExpiration, jsonMeta, function(err, result) {
  console.log(err, result);
});
```
#### Feed Publish
```
steem.broadcast.feedPublish(wif, publisher, exchangeRate, function(err, result) {
  console.log(err, result);
});
```
#### Pow2
```
steem.broadcast.pow2(wif, work, newOwnerKey, props, function(err, result) {
  console.log(err, result);
});
```
#### Fill Convert Request
```
steem.broadcast.fillConvertRequest(wif, owner, requestid, amountIn, amountOut, function(err, result) {
  console.log(err, result);
});
```
#### Fill Order
```
steem.broadcast.fillOrder(wif, currentOwner, currentOrderid, currentPays, openOwner, openOrderid, openPays, function(err, result) {
  console.log(err, result);
});
```
#### Fill Vesting Withdraw
```
steem.broadcast.fillVestingWithdraw(wif, fromAccount, toAccount, withdrawn, deposited, function(err, result) {
  console.log(err, result);
});
```
#### Interest
```
steem.broadcast.interest(wif, owner, interest, function(err, result) {
  console.log(err, result);
});
```
#### Limit Order Cancel
```
steem.broadcast.limitOrderCancel(wif, owner, orderid, function(err, result) {
  console.log(err, result);
});
```
#### Limit Order Create
```
steem.broadcast.limitOrderCreate(wif, owner, orderid, amountToSell, minToReceive, fillOrKill, expiration, function(err, result) {
  console.log(err, result);
});
```
#### Limit Order Create2
```
steem.broadcast.limitOrderCreate2(wif, owner, orderid, amountToSell, exchangeRate, fillOrKill, expiration, function(err, result) {
  console.log(err, result);
});
```
#### Liquidity Reward
```
steem.broadcast.liquidityReward(wif, owner, payout, function(err, result) {
  console.log(err, result);
});
```
#### Pow
```
steem.broadcast.pow(wif, worker, input, signature, work, function(err, result) {
  console.log(err, result);
});
```
#### Prove Authority
```
steem.broadcast.proveAuthority(wif, challenged, requireOwner, function(err, result) {
  console.log(err, result);
});
```
#### Recover Account
```
steem.broadcast.recoverAccount(wif, accountToRecover, newOwnerAuthority, recentOwnerAuthority, extensions, function(err, result) {
  console.log(err, result);
});
```
#### Report Over Production
```
steem.broadcast.reportOverProduction(wif, reporter, firstBlock, secondBlock, function(err, result) {
  console.log(err, result);
});
```
#### Request Account Recovery
```
steem.broadcast.requestAccountRecovery(wif, recoveryAccount, accountToRecover, newOwnerAuthority, extensions, function(err, result) {
  console.log(err, result);
});
```
#### Escrow Approve
```
steem.broadcast.escrowApprove(wif, from, to, agent, who, escrowId, approve, function(err, result) {
  console.log(err, result);
});
```
#### Set Withdraw Vesting Route
```
steem.broadcast.setWithdrawVestingRoute(wif, fromAccount, toAccount, percent, autoVest, function(err, result) {
  console.log(err, result);
});
```
#### Transfer
```
steem.broadcast.transfer(wif, from, to, amount, memo, function(err, result) {
  console.log(err, result);
});
```
#### Transfer To Vesting
```
steem.broadcast.transferToVesting(wif, from, to, amount, function(err, result) {
  console.log(err, result);
});
```
#### Vote
```
steem.broadcast.vote(wif, voter, author, permlink, weight, function(err, result) {
  console.log(err, result);
});
```
#### Withdraw Vesting
```
steem.broadcast.withdrawVesting(wif, account, vestingShares, function(err, result) {
  console.log(err, result);
});
```
#### Witness Update
```
steem.broadcast.witnessUpdate(wif, owner, url, blockSigningKey, props, fee, function(err, result) {
  console.log(err, result);
});
```
#### Fill Vesting Withdraw
```
steem.broadcast.fillVestingWithdraw(wif, fromAccount, toAccount, withdrawn, deposited, function(err, result) {
  console.log(err, result);
});
```
#### Fill Order
```
steem.broadcast.fillOrder(wif, currentOwner, currentOrderid, currentPays, openOwner, openOrderid, openPays, function(err, result) {
  console.log(err, result);
});
```
#### Fill Transfer From Savings
```
steem.broadcast.fillTransferFromSavings(wif, from, to, amount, requestId, memo, function(err, result) {
  console.log(err, result);
});
```
#### Comment Payout
```
steem.broadcast.commentPayout(wif, author, permlink, payout, function(err, result) {
  console.log(err, result);
});
```
#### Transfer To Savings
```
steem.broadcast.transferToSavings(wif, from, to, amount, memo, function(err, result) {
  console.log(err, result);
});
```
#### Transfer From Savings
```
steem.broadcast.transferFromSavings(wif, from, requestId, to, amount, memo, function(err, result) {
  console.log(err, result);
});
```
#### Cancel Transfer From Savings
```
steem.broadcast.cancelTransferFromSavings(wif, from, requestId, function(err, result) {
  console.log(err, result);
});
```

### Auth

#### Verify
```
steem.auth.verify(name, password, auths);
```

#### Generate Keys
```
steem.auth.generateKeys(name, password, roles);
```

#### Get Private Keys
```
steem.auth.getPrivateKeys(name, password, roles);
```

#### Is Wif
```
steem.auth.isWif(privWif);
```

#### To Wif
```
steem.auth.toWif(name, password, role);
```

#### Wif Is Valid
```
steem.auth.wifIsValid(privWif, pubWif);
```

#### Wif To Public
```
steem.auth.wifToPublic(privWif);
```

#### Sign Transaction
```
steem.auth.signTransaction(trx, keys);
``` 