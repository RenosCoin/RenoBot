# RenoBot
Renos Trading Bot

This toolkit aims to automate some trading processes, saving time and adding precision when properly calibrated.

The user is fully responsible of the outcome, it's currently at beta state, keep that in mind, we welcome any bug report so we can fix them.

Just to be clear you are fully responsible of any negative consequences from running this software even when it's a bug/doesn't work as expected.

Ping-pong
When the market movement is lateral and a divergence between the highest bid and the lowest ask in the same exchange allows you to profit by just outbidding current orders, the bot will check every 30 seconds if the criteria is still valid, and will update your current orders if necessary to outbid again, or cancel if the set up is no longer valid, and will keep waiting and checking until it's valid again, ad infinitum.

Arbitrage
Arbitrage is a well know concept, is the practice of taking advantage of a price difference between two or more markets(wikipedia) basically finds price divergences across exchanges and sell high and buy low when the criteria mets, again this will run forever until the user manually stops it or closes the bot.

The primary exchange is where you have the coins to sell, and the secondary exchange is where you expect them to buy them back at a lower price (keep in mind that you should have enough balance for the order to complete, but don't worry, in case you are missing btc for example and you can't buy back in the secondary exchange, the bot won't sell it in the primary exchange, we double check it)

When selecting multiple secondary exchanges you will notice that we merge the order books so you can see it easier, we plan to expand this concept for other features too, also the pairs are automatically checked(when opening the bot) so the dropdown list only have pairs that are present on all the selected exchanges. If it's missing at some exchange, the pair won't show up.

Whale padding

Allows to quickly set up multiple buy or sell orders so it's more organically distributed rather than manually setting up several orders.
