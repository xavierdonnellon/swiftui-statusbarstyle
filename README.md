# swiftui-statusbarstyle
Supports changing the UIStatusBarStyle with natural SwiftUI syntax. 

<h1>Usage</h1>
<h2>With new SwiftUI App Lifecycle</h2>
<b>In your App file, simply wrap your main view in a RootView.</b>

<code>
    
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
</code>
