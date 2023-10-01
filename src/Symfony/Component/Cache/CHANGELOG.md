CHANGELOG
=========

5.4
---

 * Make `LockRegistry` use semaphores when possible
 * Deprecate `DoctrineProvider` because this class has been added to the `doctrine/cache` package

5.3
---

 * added support for connecting to Redis Sentinel clusters when using the Redis PHP extension
 * add support for a custom serializer to the `ApcuAdapter` class

5.2.0
-----

 * added integration with Messenger to allow computing cached values in a worker
 * allow ISO 8601 time intervals to specify default lifetime

5.1.0
-----

 * added max-items + LRU + max-lifetime capabilities to `ArrayCache`
 * added `CouchbaseBucketAdapter`
 * added context `cache-adapter` to log messages

5.0.0
-----

 * removed all PSR-16 implementations in the `Simple` namespace
 * removed `SimpleCacheAdapter`
 * removed `AbstractAdapter::unserialize()`
 * removed `CacheItem::getPreviousTags()`
