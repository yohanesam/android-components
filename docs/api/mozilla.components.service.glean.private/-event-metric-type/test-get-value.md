[android-components](../../index.md) / [mozilla.components.service.glean.private](../index.md) / [EventMetricType](index.md) / [testGetValue](./test-get-value.md)

# testGetValue

`fun testGetValue(pingName: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)` = sendInPings.first()): `[`List`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin.collections/-list/index.html)`<`[`RecordedEventData`](../../mozilla.components.service.glean.storages/-recorded-event-data/index.md)`>` [(source)](https://github.com/mozilla-mobile/android-components/blob/master/components/service/glean/src/main/java/mozilla/components/service/glean/private/EventMetricType.kt#L124)

Returns the stored value for testing purposes only. This function will attempt to await the
last task (if any) writing to the the metric's storage engine before returning a value.

### Parameters

`pingName` - represents the name of the ping to retrieve the metric for.  Defaults
    to the either the first value in [defaultStorageDestinations](#) or the first
    value in [sendInPings](send-in-pings.md)

### Exceptions

`NullPointerException` - if no value is stored

**Return**
value of the stored metric

