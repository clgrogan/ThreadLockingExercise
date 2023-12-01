### Initial Review
    
On initial review it appears that a ReentrantReadWriteLock() methods are appropriate.

1. readLock() can be used for gets.
2. writeLock() can be used for product and review adds, deletes, and updates. Using the same lock for the review and product is appropriate.

Added the ReadWrite member variable to create the read and write objects and added the read and write members.

Updated the product add, update, and delete methods and the review add methods to return the write object.

Updated all product and review get methods to return the read object.

Copied all code within the ProductReviewsService class to the Udemy exercise IDE to run the tests.

All tests passed.
