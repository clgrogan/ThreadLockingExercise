### Initial Review
    
On initial review it appears that a ReentrantReadWriteLock() methods are appropriate.

1. readLock() can be used for gets.
2. writeLock() can be used for adds and updates. Using the same lock for the review and product is appropriate.