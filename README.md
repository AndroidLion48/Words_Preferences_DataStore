# Words App Preferences Data Store

This codelab introduces Jetpack DataStore. Built on Kotlin coroutines and Flow, DataStore provides two different implementations: Proto DataStore, which stores typed objects, and Preferences DataStore, which stores key-value pairs.



## Introduction
Words app allows you to select a letter and use Intents to navigate to an Activity that presents a number of words starting with that letter. Each word can be looked up via a web search.

Words app contains a scrollable list of 26 letters A to Z in a RecyclerView. The orientation of the RecyclerView can be changed between a vertical list or a grid of items.

The app demonstrates the use of Intents in two ways:

* to navigate inside an app by specifying an explicit destination, and,
* allowing Android to service the Intent using the apps and resources present on the device.


## Summary

- DataStore has a fully asynchronous API using Kotlin coroutines and Flow, guaranteeing data consistency.

- Jetpack DataStore is a data storage solution that lets you store key-value pairs or typed objects with protocol buffers.

- DataStore provides two different implementations: Preferences DataStore and Proto DataStore.

- Preferences DataStore does not use a predefined schema.

- Preferences DataStore uses the corresponding key type function to define a key for each value that you need to store in the DataStore<Preferences> instance. For example, to define a key for an int value, use intPreferencesKey().

- Preferences DataStore provides an edit() function that transactionally updates the data in a DataStore.


https://developer.android.com/codelabs/basic-android-kotlin-training-preferences-datastore?continue=https%3A%2F%2Fdeveloper.android.com%2Fcourses%2Fpathways%2Fandroid-basics-kotlin-unit-5-pathway-2%23codelab-https%3A%2F%2Fdeveloper.android.com%2Fcodelabs%2Fbasic-android-kotlin-training-preferences-datastore#0