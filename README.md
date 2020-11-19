# swiftui-statusbarstyle
Supports changing the UIStatusBarStyle with natural SwiftUI syntax. 

## Usage
### With new SwiftUI App Lifecycle</h2>
In your App file, simply wrap your main view in a RootView.

```swift
@main
struct ProjectApp: App {     
    var body: some Scene {
        WindowGroup {
            RootView {
                ContentView()
            }
        }
    }
}
```
