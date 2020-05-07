Single point of failure lock daemon (spoflockd)
===============================================

The spoflockd project is of questional reliability while also being questionably more reliable than a modern distributed lock manager.

This project supports long polling, websockets, callbacks, and checkin/checkout functionality.

Despite the name - spoflockd can be distributed (as shards) using modern HTTP load balancers and soft-resumption is possible.

There is no storage backend.  All locks are simple Python objects stored in dicts.
