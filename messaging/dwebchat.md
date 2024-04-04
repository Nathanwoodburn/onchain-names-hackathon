# dwebchat

## Description

dwebchat is an end to end encrypted, one to one and one to many decentralized internet relay chat (IRC) implementation. 

#### One to One

In dwebchat, everybody is a server and a client simultaneously. When user Alice messages user Bob, the following actions take place:

1. Alice retrieves Bob's IPv6 address and an EC TLS hash certificate hash from the Handshake blockchain

2. Alice retrieves the certificate from the IPv6 address.

3. Alice verifies the certificate generates a matching hash

4. If it does, Alice sends the message to Bob via a TLS channelw ith Bob's verified certificate.

#### One to Many

IRC channels are implemented as websocket servers. This is the only centralized portion of dwebchat and this decision was made based on the idea that users
consider their channels owned. This allows this to be true in the realest sense. When someone join's a channel and sends a message, for example Alice joining
# bob, the following actions take place:

1. Alice connects to a bob websocket in the root namespace of Bob

2. Alice sends a message to the bob websocket in the root namespace of Bob

3. The bob web socket relays the message to all others connected to said socket.

In dwebchat, your channels are owned by you if they are preceded by your handshake name (e.g., Bob owns #bob and #bob* where * is a wildcard matching 'anything')

#### IRC Client <-> dwebchat

dwebchat attempts to follow [RFC1459](https://datatracker.ietf.org/doc/html/rfc1459) benefiting from the vast IRC ecosystem that already exists. Any IRC client
is compatible with and works with dwebchat.

#### dwebchat Implementation Status

SERVER - Prelimary Implementation

  - Functionality:

     - WHOIS

     - JOIN

     - PART

     - NAMES

     - PRIVMSG

     - NOTICE


You can connect, get information about another user if the user's dwebchat is accessible, join and part channels, see who is in channels, and send messages to channels
and to other users.

## What needs to be developed

#### Completion of IRC protocol

dwebchat needs to implement more IRC protocol functionality in order to gain full compatibility with the wealth of features IRC brings with it. This is mainly aimed toward
IRC channel functionality (+m moderation, etc.)

#### BANG Path Routing

BANG is a concept from the old days of UUCP and the beginning of e-mail. Rather than send an e-mail to a hostname like "handshake.org," computer operators used to send e-mails to people using BANG paths.

For example, suppose I had a machine 'alice', Andrew had a machine 'bob', JJ had a machine 'charlie' and Joseph had a machine 'david'

Now, suppose I had a route to Andrew's machine from alice <-> bob, but no direct route to JJ or Joseph's machine. Suppose JJ has a route to Joseph and Andrew has a route to JJ.

Then, I could send an e-mail to Joseph like admin@bob!charlie!david

##### What about BANG?

Bringing this forward to 2024 and the advancements with civilian cryptoraphy, we can create an 'onion' like routing system wherein hops are obscured from anyone attempting to intercept and inspect transactions.

By utilizing the prime256v1 public/private keypair generated for TLS, ECDH can be utilized to derive a shared secret key and further, secretly and safely exchange temporary and ephemeral keys go forward.

Thus, an onion style routing mechanism can be created wherein each hop can decrypt the next hop to know where to send, but only the next hop.

Further, extra hops can be placed within a MAX_HEADER_SIZE amount of space which should be defined by the protocol, thus giving deniability to who or where a message was sent.

Thus, I could send a message to 'cory' through a bunch of other names like this:

```
joe!david!andrew!joseph!cory!jj!steven
```

Even though I sent a message to cory, the message continued to be sent all the way to steven. There is no telling who actually received the message and was able to decrypt it.

Further, only I know the full path. david only knows to send to andrew. andrew only knows to send to joseph, and so on. Additionally, they will not know who sent the original message as ephemeral public keys should be used on sender's side to conceal this information.

##### How does this help?

Adding this feature in increases the security and privacy of the dwebchat system considerably.

Right now, signal and telegram know who you are talking to, at what time, and generally have a good idea on the size of your messages. Even this metadata can be concealed in dwebchat.


## Links

- [dwebchat](https://github.com/realrasengan/dwebchat)
