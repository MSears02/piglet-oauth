# piglet-oauth

The OAuth return page for [Piglet](https://github.com/MSears02/Piglet), published with GitHub Pages at
https://msears02.github.io/piglet-oauth/.

Banks that sign in on their own site through Plaid (Capital One, Chase, ...) send you back to this page
when you're done. In a desktop browser that's a pop-up, and Plaid finishes in Piglet's window by itself;
otherwise the page forwards you to Piglet on your own computer (`http://localhost:8765/oauth`), passing
along the bank's one-time `oauth_state_id`. It stores nothing and sends nothing anywhere else.

To use it, add the address above under **Allowed redirect URIs** in Plaid's Dashboard, and as the
**OAuth return page** in Piglet (Accounts page, Plaid keys...).
