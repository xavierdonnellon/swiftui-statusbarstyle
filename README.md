# swiftui-statusbarstyle
Supports changing the UIStatusBarStyle with natural SwiftUI syntax. 

<h1>Usage</h1>
<h2>With new SwiftUI App Lifecycle</h2>
In your App file: 
<code>
    @main
    struct ProjectApp: App {
        //The view you want your app to start on 
        var rootView: some View {
            ContentView()
            //add any necessary environment objects here 
        }

        var body: some Scene {
            WindowGroup {
                EmptyView()
                    .onAppear {
                        UIApplication.shared.setHostingController(rootView: AnyView(self.rootView))
                    }
            }
        }
    }
</code>
