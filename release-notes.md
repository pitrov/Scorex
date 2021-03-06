**1.2.0**
---------

* Web interface to core API has been added. Please set "rpcport" value in settings.json then visit
   http://localhost:{rpcport}/ after server bootstrapping.

* Permacoin implementation has been added. Permacoin is blockchain consensus protocol based on
non-interactive Proof-of-Retrievability of a static dataset by A. Miller, E. Shi, J. Katz, B. Parno et at.
 For details please see the paper http://cs.umd.edu/~amiller/permacoin.pdf . Protocol settings could be changed
 in perma.conf.

* For Permacoin module, new API calls are /consensus/target, /consensus/target/{blockId},
 /consensus/puz, /consensus/puz/{blockId} .

* P2P layer is totally rewritten. From now a new module can implement messages and messages handling
logic separately. Then module p2p logic is to be wired into application's logic.

* Experimental: a node could store a blocktree explicitly. Storage type could be changed via "history"
setting(set "blockchain" / "blocktree"). Different nodes can have different storage types.


**1.1.2**
---------

* API call added: consensus/algo

* API calls added for Qora-like consensus algo: consensus/time, consensus/time/{generatingBalance}, 
 consensus/generatingbalance, consensus/generatingbalance/{blockId}

* API calls added for Nxt-like consensus algo: consensus/basetarget, consensus/basetarget/{blockId},
  consensus/generationsignature, consensus/generationsignature/{blockId}

**1.1.1**
---------

* API call added: addresses/sign
* API call added: addresses/create
* API call added: DELETE to addresses/address/{address}
* Less buggy blockchain synchronization logic


**1.1.0**
----------

* Modular design: basics, consensus, transaction modules are extracted
* Ping messages removed
* Docker container


**1.0.4**
---------

* Scorex-crypto module has been extracted as the separate sub-project


**1.0.3**
---------

* This file has been started :) 

* SBT commands instead of linux shell scripts   

 
