# swiftui-statusbarstyle
Supports changing the UIStatusBarStyle with natural SwiftUI syntax. 

## Usage
### With new SwiftUI App Lifecycle</h2>
In your @main App file, simply wrap your main view in a RootView.

```swift
@main
struct ProjectApp: App {     
    var body: some Scene {
        WindowGroup {
            RootView {
                //Put the view you want your app to present here
                ContentView()
                    //Set the status bar style here
                    .statusBarStyle(.lightContent)
            }
        }
    }
}
```

### With AppDelegate / SceneDelegate Lifecycle
In your SceneDelegate.swift file, 
