# Victoria Tran 
# CWID: 889773024
# CS 411 MIDTERM 
#This is part 2 of the coding portion of the exam. Coding Portion Part 1 is in the main.swift 

---------------------------------------------------


# Question 1
```swift

struct ContentView: View {
 var body: some View {
  Text("I'm an iOS Developer!")
    .padding()
    .background(Color.red)
    .padding()
    .background(Color.blue)
    .padding()
    .padding()
    .background(Color.green)
   }
 }

```
# Question 2
```swift

struct ContentView: View {
  var body: some View {
    Button("Live long and prosper")
      .frame(width: 200, height: 200)
      .background(Color.red)
     }
  }

```
# Question 3
```swift

struct ContentView: View {
  var body: some View {
    NavigationBar{
      Form {
        Section {
          Text("Hello, world!");
          Text("Hello, world!");
         }
         Section { 
          Text("Hello,world!");
          Text("Hello,world!");
         }
  Section { 
          Text("Hello,world!");
         }}.navigationBarTitle("SwiftUI")
        }
       }
      }
     }
  



```
# Question 4
```swift

struct ContentView: View {
@State private var showingAlert = false
var body: some View {

  Button("Show Alert: ") {
    self.tapCount += 1
    self.showingAlert = true
  }
  
  .alert(isPresented: $showingAlert) {
    Alert(title: Text("Tapcount"), message: Text("\(self.tapCount)"),
        dismissButton: .default(Text("OK")))
    }
   }
  }


```
