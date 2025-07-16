# RBXAntiBackshot
A system to help you take action against a prevalent behavior in Roblox games wherein one user presses W and S behind another player, thus looking like they're giving them "backshots".

This behavior is highly problematic due to the fact that it is inherently a sexual innuendo, which is not only prohibited by Roblox Terms of Service, but additionally the person on the receiving end typically is not friends with the person doing it or otherwise okay with this behavior.

(Files are currently not hosted on GitHub, they will be when I deem this system ready!)

## Implementation Details
As of right now (7/15/2025) implementation is mostly finished, there's just some stuff I want to improve and additions I want to make before releasing this to the broader public.

Here's the basic run down of what I've got so far:
- Backshot detection that works based on spatial queries, HRP Velocity, and MoveDirection.
- False positives are impossible due to the design of the detection, and false negatives are unlikely.
- Completely server sided, though a client component may be added in the future.
- Configurable with many settings to optimize sensitivity and performance.
- BindableEvent that you can connect to so you may enable your own actioning behavior.
- Protect your NPCs through a CollectionService tag.
- Performance is pretty fast, 500 NPCs still run at 60TPS.

Designing this thus far has been a balancing act between performance and accuracy, I'm basically done as far as accuracy goes, there's nothing more that really needs to be done there, but for performance, there's a few more things I'd like to do before I consider this "finished". I may also extend this system to "frontshotting" as well.
