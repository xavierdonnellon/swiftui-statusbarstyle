# swiftui-statusbarstyle
Supports changing the UIStatusBarStyle with natural SwiftUI syntax. 

## Usage
### With new SwiftUI App Lifecycle</h2>
In your```swift @main``` App file, simply wrap your main view in a RootView.

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
In your ```SceneDelegate.swift```, in your```swift scene``` function, simply wrap your main view in a ```RootView```. 
```swift
class SceneDelegate: UIResponder, UIWindowSceneDelegate {

    var window: UIWindow?

    func scene(_ scene: UIScene, willConnectTo session: UISceneSession, options connectionOptions: UIScene.ConnectionOptions) {

        // Create the SwiftUI view that provides the window contents.
        let contentView = ContentView()
            .environmentObject(TestObject())

        // Use a UIHostingController as window root view controller.
        if let windowScene = scene as? UIWindowScene {
            let window = UIWindow(windowScene: windowScene)
            window.rootViewController = UIHostingController(rootView: RootView { contentView.statusBarStyle(.lightContent) })
            self.window = window
            window.makeKeyAndVisible()
        }
    }
    
    //rest of default SceneDelegate goes unchanged...

