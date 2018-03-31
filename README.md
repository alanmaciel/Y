# Y

Y is a new way to fund public services: you choose which services are funded, and where they are funded (i.e. not just in your own country, but anywhere in the world). There are no tax returns to do.

Y could raise enough money to take over from the tax system, and let enough people decide how public money should be spent to take over from centralised government. Enough money could cross national borders that national borders would be obsolete. With no countries, there can be no wars between them. I believe Y may be a solution for world peace.

## How it works

Rather than waiting for a seller (say, a global corporation) to make sales before taxing them, Y takes tax (actually, a voluntary donation set by the seller) from the sale. The more a seller chooses to donate from the sale, the more sales they'll make. The buyer/global citizen sets what the donation will go to.

As it stands, Y is a smart contract that handles this process out in the open (on the blockchain), so neither the buyer nor the seller have to trust each other to make the donation. The same idea could be implemented by a bank, but then you'd have to trust the bank, and hope that it'd stay in business.

## Development

Right now, Y is an Ethereum smart contract. That may change as better blockchains arrive.

There are two layers: the core smart contract, written in Solidity, and the interface around it, so that it's nicer to use (for example, Solidity doesn't work with decimals, so the interface changes them to a numerator and denominator). The interface happens to be written in JavaScript, so that it can be called from a web app, but it could be written in any language that calls Ethereum.

This project practises test-driven development. I'm also investigating formal methods, like [K](https://runtimeverification.com/blog/?p=496), so that we can prove properties of the contract for higher assurance. The project is part of [AgileVentures](https://www.agileventures.org/projects/y), and we mob program on it every [Thursday at 5pm UTC](https://www.agileventures.org/events/y-mob-programming). If you'd like to work on it now, contact me through Y's channel on AgileVentures' Slack.

### Plan right now

Prove that Ether can't get stuck in the contract via the payAndDonate function, or mitigate this problem with a function to return stuck Ether to the payer.

Find sellers who are already accepting Ether, and ask them if they'd like to use Y.
