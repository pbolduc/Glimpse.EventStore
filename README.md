Glimpse.EventStore
==================

Glimpse (http://getglimpse.com/) plugin for Event Store (http://geteventstore.com).

Plugin adds an 'Event Store' tab to Glimpse client that displays all activity on EventStore connection, including duration, arguments and results.

Usage
=====

1. Add Glimpse.EventStore package to the project where you create an instance of `IEventStoreConnection`,
2. Replace calls to `EventStore.ClientAPI.EventStoreConnection.Create(...)` with `Glimpse.EventStore.ProfiledEventStoreConnection.Create(...)`. `ProfiledEventStoreConnection` has exactly the same `Create` methods as `EventStoreConnection`. 

No other changes in the code are needed.

Roadmap
=======

Features to implement:

1. Optionaly hiding `UserCredentials.Password` field,
2. Proper timings for async methods (currently timings show only the duration of returning a `Task` instance, not the actual execution of the `Task`),
3. Deserialization of individual events' body and metadata,
4. Improvements in the UI.

Disclaimer
==========

This is an alpha version of the plugin. May contain bugs.
If you're lucky to find one, please report it on GitHub.

Also, do not withhold any suggestions or feedback.
