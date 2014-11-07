iCloudCoreData-Swift
====================

Based on https://github.com/mluisbrown/iCloudCoreDataStack - Kudos! 
Swift version from Xcode generated code + some help from Apple Technical support - let's make it better together

USAGE:
In AppDelegate.swift, add a member var:
  var persistentStack: PersistentStack?
In didFinishLaunchingWithOptions, init then assign to whatever class managedObjectContext belongs to:
  persistentStack = PersistentStack()
  rootVC.managedObjectContext = persistentStack?.managedObjectContext
In applicationWillResignActive etc, to save context:
  persistentStack?.saveContext()
  
This is based on my shallow knowlege - please let me know of any issues you find!
