# swiftui-statusbarstyle
Supports changing the UIStatusBarStyle with natural SwiftUI syntax. 

<h1>Usage</h1>
<h2>With new SwiftUI App Lifecycle</h2>
<b>In your App file:</b>

<code>
    @main
struct DatingApp: App {
    
    @UIApplicationDelegateAdaptor(AppDelegate.self) var appDelegate
    
    var body: some Scene {
        WindowGroup {
            RootView {
                ContentView()
            }
        }
    }
}
</code>
